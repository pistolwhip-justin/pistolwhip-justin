[  
Freedium](https://freedium.cfd/)

- [ko-fi](https://ko-fi.com/zhymabekroman)
- [librepay](https://liberapay.com/ZhymabekRoman/)
- [patreon](https://patreon.com/Freedium)

[< Go to the original](https://towardsdatascience.com/introducing-the-new-anthropic-token-counting-api-5afd58bad5ff#bypass)

![Preview image](https://miro.medium.com/v2/resize:fit:700/1*8qT5lxqBEKoQYJsIO6yPPQ.png)

# Introducing the New Anthropic Token Counting API

## Keep a closer eye on your costs when using Claude

[![Thomas Reid](https://miro.medium.com/v2/resize:fill:88:88/1*9HLVlE34bSbCDExHKmVpvg.jpeg)

](https://medium.com/@thomas_reid "A data engineer , specialising in the AWS cloud with particular interest in AI, serverless and the energy, finance and insurance sectors")

[Thomas Reid](https://medium.com/@thomas_reid "A data engineer , specialising in the AWS cloud with particular interest in AI, serverless and the energy, finance and insurance sectors")[Follow](https://medium.com/@thomas_reid "A data engineer , specialising in the AWS cloud with particular interest in AI, serverless and the energy, finance and insurance sectors")

[![Towards Data Science](https://miro.medium.com/v2/resize:fill:48:48/1*CJe3891yB1A1mzMdqemkdg.jpeg)

Towards Data Science

](https://medium.com/towards-data-science "Your home for data science.")androidstudio~9 min read·November 8, 2024 (Updated: November 8, 2024)·Free: No

Anthropic has released some exciting beta features in the last couple of days that have largely gone under the radar. One of these was the ability to process PDFs with their models, which can now understand both text and visual content within PDF documents. I'll maybe write up something on that at a later date.

The other exciting beta feature, and the subject of this article, was the introduction of token counting. Crucially, you can count the tokens in user messages, PDFs and images _**before**_ you send them to Claude. This is excellent news for those who like to monitor their token usage costs closely.

According to the official announcement from Anthropic (link [here](https://docs.anthropic.com/en/docs/build-with-claude/token-counting)),

> "The token counting endpoint accepts the same structured list of inputs for creating a message, including support for system prompts, tools, images, and PDFs. The response contains the total number of input tokens."

And supports the following models,

> "Claude 3.5 Sonnet Claude 3.5 Haiku Claude 3 Haiku Claude 3 Opus"

The good news is that token counting is free to use but subject to requests per minute rate limits based on your usage tier.

For the rest of this article, we'll go through some examples of using the token counting API to count tokens in user/system messages, PDFs and images.

To make things more interactive, once we have the basics of our code developed, we'll wrap up the functionality in a Gradio app that will display a nice user interface to enter user text or upload PDFs and images, then count the tokens. It'll look a bit like this,

![None](https://miro.medium.com/v2/resize:fit:700/1*tq9BRCXyrSv-xsk6fEuEUw.png)

Image by Author

Ok, let's get started. First off, I'm developing using Windows WSL2 Ubuntu. If you're a Windows user, I have a comprehensive guide on installing WSL2, which you can find [here](https://medium.com/stackademic/installing-wsl2-ubuntu-for-windows-81122c551bc2).

#### Setting up a dev environment

Before we start coding, let's set up a separate development environment. That way, all our projects will be siloed and won't interfere with each other. I use conda for this, but use whichever tool you're familiar with.

Copy`(base) $ conda create -n token_count python=3.10 -y (base) $ conda activate token_count # Install required Libraries (token_count) pip install anthropic jupyter`

#### Getting an Anthropic API key

You can get that from the [Anthropic Console](https://console.anthropic.com/). Register or Sign-In, then you'll see a screen like this,

![None](https://miro.medium.com/v2/resize:fit:700/0*zBAzmZH9yezP39un.png)

Image from Anthropic Website

Click the **`Get API Keys`** button and follow the instructions from there. Take note of your key and set the environment variable ANTHROPIC_API_KEY to it.

#### The code

Example 1 — Counting tokens in the user and system prompts.

Copy`import anthropic import os  client = anthropic.Anthropic()  response = client.beta.messages.count_tokens(     betas=["token-counting-2024-11-01"],     model="claude-3-5-sonnet-20241022",     system="""         You are a helpful assistant and will respond to users's queries          in a polite, friendly and knowledgable manner     """,     messages=[{         "role": "user",         "content": "What is the capital city of France"     }], )  print(response.json())  # # Output #  {"input_tokens":41}`

Example 2— Counting tokens in a PDF

For my input PDF, I'll use a copy of Tesla's Q10 September 2023 quarterly submission to the Securities and Exchange Commission. This document is 51 pages of mixed text and tabular data. You can see what it looks like online by clicking [here](https://www.sec.gov/Archives/edgar/data/1318605/000162828023034847/tsla-20230930.htm).

Copy`import base64 import anthropic  client = anthropic.Anthropic()  with open("/mnt/d/tesla/tesla_q10_sept_23.pdf", "rb") as pdf_file:     pdf_base64 = base64.standard_b64encode(pdf_file.read()).decode("utf-8")  response = client.beta.messages.count_tokens(     betas=["token-counting-2024-11-01", "pdfs-2024-09-25"],     model="claude-3-5-sonnet-20241022",     messages=[{         "role": "user",         "content": [             {                 "type": "document",                 "source": {                     "type": "base64",                     "media_type": "application/pdf",                     "data": pdf_base64                 }             },             {                 "type": "text",                 "text": "Please summarize this document."             }         ]     }] )  print(response.json())  # # Output #  {"input_tokens":118967}`

Example 3 — Counting tokens in an image

This is the image I'll use.

![None](https://miro.medium.com/v2/resize:fit:700/1*Ndhggt29pRXXzCOTykywbQ.png)

Image by AI (Dalle-3)

It's a PNG and approximately 2.6MB in size.

Copy`import anthropic import base64 import httpx  image_url = "/mnt/d/images/android.png" image_media_type = "image/png" # Read the image file and encode it to base64 with open(image_path, "rb") as image_file:     image_data = base64.standard_b64encode(image_file.read()).decode("utf-8")  client = anthropic.Anthropic()  # Create the request using the locally stored image response = client.beta.messages.count_tokens(     betas=["token-counting-2024-11-01"],     model="claude-3-5-sonnet-20241022",     messages=[         {             "role": "user",             "content": [                 {                     "type": "image",                     "source": {                         "type": "base64",                         "media_type": image_media_type,                         "data": image_data,                     },                 },                 {                     "type": "text",                     "text": "Describe this image"                 }             ],         }     ], )  print(response.json())  # # Output #  {"input_tokens":1575}`

Note that in all the above examples, no requests were set to the LLM to answer any user questions. It was just token counting.

#### Pulling it all together into a Gradio app.

Now that we have all the code we need, let's design a user interface for it using Gradio.

We need two input text boxes, one for an optional system prompt and one for an optional user prompt.

Next, we'll need an input field where the user can select PDF or image files to upload. Below this field, there will be a **`Add`** button to allow the user to add the files chosen above. The names of any chosen files or images will be displayed in a message box.

Finally, there will be a button that calls the code to calculate the token cost and a button to clear all input and output fields.

We can do this part using an LLM. It took a bit of back and forth with the LLM, but eventually, with GPT4-o's help, I developed this code. It's heavily commented on, so it should be relatively easy to follow.

Copy`# Import Gradio for building the web app interface import gradio as gr # Import Anthrop client for token counting API import anthropic # Import base64 for encoding files in base64 format import base64 # Import os for interacting with the file system (though not used in this script) import os  # Initialize the Anthropic client to access the API functions # need to have your ANTHROPIC_API_KEY environment variable set client = anthropic.Anthropic()  # Define a function to handle file uploads incrementally, allowing files to be added without overwriting previous uploads def add_files(uploaded_files, current_files):     # Initialize the current_files list if it's empty     if current_files is None:         current_files = []          # Append any newly uploaded files to the current list of files     if uploaded_files:         current_files.extend(uploaded_files)          # Create a list of file names for display purposes     file_names = [file.name for file in current_files]          # Return the updated file list, the display names, and clear the uploaded_files input     return current_files, file_names, None  # Define a function to count tokens in system and user prompts, as well as in uploaded files def count_tokens(system_prompt, user_prompt, all_files):     # Check if all inputs are empty or cleared; if so, return 0     if not system_prompt and not user_prompt and not all_files:         return 0      # Initialize an empty list to store the message objects for the API request     messages = []          # Add the user prompt to the messages list if it's provided     if user_prompt:         messages.append({             "role": "user",             "content": user_prompt         })          # Process each uploaded file, determining whether it's a PDF or an image     if all_files:         for file in all_files:             # Get the file type by extracting and converting the file extension to lowercase             file_type = file.name.split(".")[-1].lower()                          # If the file is a PDF, encode it in base64 and prepare a document message             if file_type == "pdf":                 with open(file.name, "rb") as f:                     pdf_base64 = base64.standard_b64encode(f.read()).decode("utf-8")                 pdf_content = {                     "type": "document",                     "source": {                         "type": "base64",                         "media_type": "application/pdf",                         "data": pdf_base64                     }                 }                 # Add the PDF message to the messages list with a prompt for summarization                 messages.append({                     "role": "user",                     "content": [pdf_content, {"type": "text", "text": "Please summarize this document."}]                 })                          # If the file is an image (JPEG or PNG), encode it in base64 and prepare an image message             elif file_type in ["jpg", "jpeg", "png"]:                 media_type = f"image/{file_type}"                 with open(file.name, "rb") as f:                     image_base64 = base64.standard_b64encode(f.read()).decode("utf-8")                 image_content = {                     "type": "image",                     "source": {                         "type": "base64",                         "media_type": media_type,                         "data": image_base64,                     }                 }                 # Add the image message to the messages list with a prompt to describe it                 messages.append({                     "role": "user",                     "content": [image_content, {"type": "text", "text": "Describe this image"}]                 })          # If no prompts or files are provided, add a placeholder message     if not messages:         messages.append({             "role": "user",             "content": "\0"         })          # Call the Anthrop API to count tokens, using system prompt and messages as input     response = client.beta.messages.count_tokens(         betas=["token-counting-2024-11-01", "pdfs-2024-09-25"],         model="claude-3-5-sonnet-20241022",         system=system_prompt,         messages=messages,     )          # Return the total number of tokens counted     return response.input_tokens  # Define a function to clear all input fields in the Gradio app def clear_inputs():     return "", "", [], "", ""  # Build the Gradio interface with gr.Blocks(theme="huggingface") as app:     # Display a title for the app     gr.Markdown("<h1 style='text-align: center;'>Anthropic Token Counter</h1>")          # Create input fields for system and user prompts     with gr.Row():         system_prompt = gr.Textbox(label="System Prompt", placeholder="Enter the system prompt here...", lines=3)         user_prompt = gr.Textbox(label="User Prompt", placeholder="Enter the user prompt here...", lines=3)          # Create an upload field for multiple PDF or image files     uploaded_files = gr.File(label="Upload PDF(s) or Image(s)", file_count="multiple", file_types=[".pdf", ".jpg", ".jpeg", ".png"])          # Create a state variable to hold the list of currently uploaded files     current_files = gr.State([])          # Display a text box to show the names of uploaded files     file_display = gr.Textbox(label="Uploaded Files", interactive=False)       # Define buttons for adding files, counting tokens, and clearing inputs     add_files_button = gr.Button("Add Files")     with gr.Row():         count_button = gr.Button("Count Tokens", size="small")         clear_button = gr.Button("Clear", size="small")              # Display the token count result in a text box     result = gr.Textbox(label="Token Count", interactive=False)          # Configure the "Add Files" button to append files to the current file list     add_files_button.click(fn=add_files, inputs=[uploaded_files, current_files], outputs=[current_files, file_display, uploaded_files])      # Configure the "Count Tokens" button to process the prompts and files, displaying the token count     count_button.click(fn=count_tokens, inputs=[system_prompt, user_prompt, current_files], outputs=result)      # Configure the "Clear" button to reset all inputs and the token count display     clear_button.click(fn=clear_inputs, outputs=[system_prompt, user_prompt, current_files, file_display, result])  # Launch the Gradio app app.launch()`

To use the app, do the following.

- Enter a system and/or user prompt if required. You can leave these blank if you want.
- To upload one or more files, drag a file into the file upload box or click on it and choose a file. After this, click the **Add** button, and your chosen file should appear in the **Uploaded Files** list box.
- Repeat the step above to add more files if you want
- Click the **Count Tokens** button to display a count of the tokens in all uploaded files and/or any text entered into the user or system prompts
- Click the **Clear** button to reset everything and start from scratch

Here's an example run where I uploaded 2 PDF files and an image along with a user prompt.

![None](https://miro.medium.com/v2/resize:fit:700/1*3cowWkZelGhcg9UNAfLBQQ.png)

Image by Author

#### Summary

In this article, I wrote about an announcement made by Anthropic about a new token-counting API that had been released in beta. I then went on to use the API to develop code that counts tokens for user and system prompts, as well as for uploaded images and PDF documents.

I then showed how you would develop a user interface for the code using Gradio, bundling the code we developed into the app.

Finally, I showed what the app looks like and provided a working example of its use.

> _Ok, that's all for me for now. Hopefully, you found this article useful. If you did, please check out my profile page at_ _[this link](https://medium.com/@thomas_reid)__. From there, you can see my other published stories and subscribe to get notified when I post new content._

> _I know times are tough and wallets constrained, but if you got real value from this article, please consider_ _[buying me a wee dram](https://ko-fi.com/taupirho)__._

If you liked this content, I think you'll find these articles interesting, too.

[

## Develop, then deploy a WEBP to PNG image converter Taipy App to the web — Part 1

### Developing the App

gopubby.com



](https://ai.gopubby.com/develop-then-deploy-a-webp-to-png-image-converter-app-to-the-web-part-1-0ed2ed6227ce)

[

## C Programming Using Claude’s New Computer Use Model

### How well can Sonnet write and run code on your behalf?

towardsdatascience.com



](https://towardsdatascience.com/c-programming-using-claudes-new-computer-use-model-feaad7e3e8db)

[#data-science](https://medium.com/tag/data-science "Data Science")[#data-engineering](https://medium.com/tag/data-engineering "Data Engineering")[#llm](https://medium.com/tag/llm "Llm")[#artificial-intelligence](https://medium.com/tag/artificial-intelligence "Artificial Intelligence")[#claude-ai](https://medium.com/tag/claude-ai "Claude Ai")

![](chrome-extension://cakobppopkpmmglabcdcklncbckjpkcl/assets/logo.png)

Ctrl+M

![Apollo](data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggZD0iTTE4LjYwMDUgNS42NzMzM0gxNS41MzYxTDE3LjEyNTEgOC4zOTY4MkwxOC42MDA1IDUuNjczMzNaIiBmaWxsPSJibGFjayIvPgo8cGF0aCBkPSJNMjIuODU5MyAyMS4wNDdMMTEuOTgxMSAyLjk0OTg0TDEuMTM5MTkgMjEuMDA5MUg2Ljk0NTkzQzcuNzIwNjkgMjEuMDA5MSA4LjQ4MjgzIDIwLjgxMzUgOS4xNTY2IDIwLjQ0MjdDOS44ODQwMiAyMC4wNDE5IDEwLjQzMzEgMTkuNDYxMiAxMC44NjIzIDE4Ljc1NzRDMTEuMzY0MSAxNy45MzM4IDExLjg1MTcgMTcuMTAwNiAxMi4zNDU2IDE2LjI3MjJMMTMuNjA5NSAxNC4xNTE1TDExLjk3OTUgMTEuNDIwMUwxMS4yNTY4IDEyLjU4M0MxMC40MzMxIDEzLjk2MDYgOS42NTM2NCAxNS4zNjk2IDguNzk5OTkgMTYuNzI4MkM4LjM3MDggMTcuNDA5OSA3LjgxMDYzIDE4LjA1MzcgNi45ODM4IDE4LjIxOTRDNi44NTkxNSAxOC4yNDQ2IDYuNzMxMzQgMTguMjU3MiA2LjYwMzUzIDE4LjI2MkM2LjQzMzExIDE4LjI2ODMgNi4yNjI3IDE4LjI2NTEgNi4wOTM4NiAxOC4yNjUxTDExLjk4MTEgOC4yMzkwM0wxOS41NDA5IDIxLjA0N0gyMi44NTkzWiIgZmlsbD0iYmxhY2siLz4KPC9zdmc+Cg==)