---
aliases:
  - Can You Automate Everything with an AI Agent? Here's How I Did It
---
![Preview image](https://miro.medium.com/v2/resize:fit:700/0*CB-GjCiH_wQsdnt8.png)

# Can You Automate Everything with an AI Agent? Here's How I Did It

## "You ever wish you had an assistant who could just handle all the little stuff? Checking your emails, managing your calendar, following up…

[![Singh Manpreet](https://miro.medium.com/v2/resize:fill:88:88/1*YaViKfuc2uAV4OhpLOsZXw.jpeg)

](https://medium.com/@singh.manpreet171900 "Data Scientist | AI | Machine Learning |Research & Technical Writer Connect with me on LinkedIn to collaborate : https://www.linkedin.com/in/manpreet17/")

[Singh Manpreet](https://medium.com/@singh.manpreet171900 "Data Scientist | AI | Machine Learning |Research & Technical Writer Connect with me on LinkedIn to collaborate : https://www.linkedin.com/in/manpreet17/")[Follow](https://medium.com/@singh.manpreet171900 "Data Scientist | AI | Machine Learning |Research & Technical Writer Connect with me on LinkedIn to collaborate : https://www.linkedin.com/in/manpreet17/")

[![AI Advances](https://miro.medium.com/v2/resize:fill:48:48/1*R8zEd59FDf0l8Re94ImV0Q.png)

AI Advances

](https://medium.com/ai-advances "Democratizing access to artificial intelligence")androidstudio~8 min read·October 10, 2024 (Updated: October 11, 2024)·Free: No

> "You ever wish you had an assistant who could just handle all the little stuff? Checking your emails, managing your calendar, following up with people — basically all the things that take up your time but don't need you to do them. Well, I did too. So I decided to build one. And the best part? I did it with no-code tools, and you can too."

Have you ever wished for a personal assistant who could handle all your mundane tasks by keep you organized and save you precious time?

Well, I recently went on a journey to create exactly that — a no-code team of AI personal agents that can do just about anything. From managing your calendar and email inbox to updating your CRM or project management tool, sending emails and even creating meetings with desired guests. This AI agent can handle it all.

In this article, I'll walk you through how I built this AI assistant step by step using a no-code platform called **n8n**. Whether you're a business owner looking to streamline operations or just someone eager to automate daily tasks, this guide is for you. Let's dive in!

**Why I Built This AI Assistant**

Before we get into the nuts and bolts, let me share a bit of the backstory. I recently started exploring n8n, a powerful no-code automation platform, and I wanted to test its capabilities by building something complex yet practical. The idea of an AI assistant that could handle personal administration tasks seemed like the perfect challenge.

The tasks this agent can perform are not just gimmicks; they genuinely save time and help you stay informed. By automating repetitive tasks, you free up mental space to focus on what truly matters.

**What This AI Assistant Can Do**

- **Manage Your Calendar**: Get summaries of your schedule for today, tomorrow, next week, or even next month.
- **Handle Emails**: Summarize emails received on any given day.
- **Update CRM or Project Management Tools**: Create tasks, update records, and keep everything in sync.
- **Send Emails**: Compose and send emails through voice commands or text messages.
- **Create Meetings and Events**: Schedule meetings in your calendar and invite guests automatically.

And the best part? You can interact with this assistant through simple text messages or even voice commands using Siri!

I personally love the convenience of just saying,

_**"Hey Siri, ask my AI assistant to get my emails from yesterday."**_

Within moments, I receive a summarized version of my inbox, saving me from the time-consuming task of checking through each email. I even asked it to schedule a meeting with a friend, saying something like

_"Can you set up a meeting with Rahul for Thursday at 1 PM?"_

Minutes later, my calendar was updated, and Rahul received the invitation.

**Getting Started: Tools You'll Need**

Before we begin, here's a list of tools and accounts you'll need:

1. **n8n Account**: Sign up at n8n.io.
2. **Twilio Account**: For sending and receiving SMS messages. Sign up at twilio.com.
3. **OpenAI API Key**: To use GPT models for natural language understanding. Get yours at openai.com.
4. **Gmail Account**: For email functionalities.
5. **Google Sheets**: Acting as a simple CRM.
6. **Notion Account**: For project management tasks.
7. **Google Calendar**: To manage and create events.

**Step 1: Setting Up Twilio for SMS Communication**

First things first, we need a way to communicate with our AI assistant. I chose Twilio because it allows us to send and receive SMS messages, and it's easy to integrate with n8n.

**Purchase a Twilio Number**

- Sign up for a Twilio account.
- Purchase a phone number capable of sending and receiving SMS messages. This usually costs around $1 per month.

**Connect Twilio to n8n**

- In your n8n workflow, add a new node and select Twilio.
- Choose "Trigger on New SMS" as the event.
- Enter your Twilio credentials (Account SID and Auth Token).
- Set the phone number to the one you just purchased.

Now, whenever you send a text message to your Twilio number, it will trigger the n8n workflow. For example, while driving, I use Siri to send a quick voice command like, _"Hey Siri, text my AI assistant to get my calendar for next week."_ Moments later, I get an SMS back with my full schedule.

**Step 2: Processing Messages with OpenAI**

Our AI assistant needs to understand what we're asking. This is where OpenAI's GPT models come into play.

**Add OpenAI Node to Your Workflow**

- After the Twilio trigger node, add an OpenAI node.
- Configure it to use the ChatGPT model.

**Crafting the Prompt**

We need to guide the AI on how to interpret our messages. Here's the prompt I used:

Copy`Your task is to analyze the message and decide which actions to take. There are five possible actions, and your output should be based on the content of the message and apply common sense to determine the correct actions. The five actions are: 1. Get Calendar 2. Get Emails 3. Create Task 4. Send Email 5. Create Meeting Important: Your output should only contain the actions that are directly relevant to the message. Examples: - If the message says, "Please send me the emails from last week," your output should be: Get Emails - If the message says, "We need to set up a meeting for tomorrow," your output should be: Create Meeting - If the message says, "Can you check my schedule and send a follow-up email," your output should be: Get Calendar, Send Email Analyze the following message: {{Your Message Here}} Use common sense and logic to decide the correct actions based on the message.`

This prompt tells the AI to analyze incoming messages and decide what action or actions are needed.

**Testing the OpenAI Node**

- Try sending different messages to your Twilio number and see if the OpenAI node correctly identifies the required actions. For example:

> _"Can you get my emails from yesterday?"_

> _"Schedule a meeting with John Doe next Monday at 10 AM."_

**Step 3: Routing Actions with IF Nodes**

Now that the AI can identify the required actions, we need to route the workflow accordingly.

- **Add IF Nodes for Each Action**
- **Get Emails IF Node**: Condition — If OpenAI output contains "Get Emails".
- **Send Email IF Node**: Condition — If OpenAI output contains "Send Email".
- **Get Calendar IF Node**: Condition — If OpenAI output contains "Get Calendar".
- **Create Task IF Node**: Condition — If OpenAI output contains "Create Task".
- **Create Meeting IF Node**: Condition — If OpenAI output contains "Create Meeting".

These nodes ensure that only the relevant actions are executed based on the user's message.

**Step 4: Implementing Each Action**

**A. Get Emails**

**Determine the Date Range**

- Add another OpenAI node to extract the date or time frame from the message.

Copy`Determine the date range for the emails to retrieve.  Message: {{Your Message Here}} Current Date: {{Current Date}}  Instructions: - If the message says "today," output today's date. - If it says "yesterday," output yesterday's date. - For "last week," calculate the date range for the last seven days.`

**Fetch Emails from Gmail**

- Add a Gmail node.
- Set it to "List Emails".
- Use the date range from the previous step to filter emails.

**Send Email Summaries via Twilio**

- Add a Twilio node.
- Compose a message that includes summaries or snippets of the emails.
- Send the message to your phone number.

**B. Send Email**

**Extract Recipient and Message Content**

- Use OpenAI to parse the recipient's name and the email body from your message.

Copy`Extract the recipient's name and the email body from the following message.  Message: {{Your Message Here}}  Output: Recipient Name: [Name] Email Body: [Body]`

**Lookup Email Address in Google Sheets**

- Add a Google Sheets node.
- Use the recipient's name to search your CRM sheet and retrieve the email address.

**Compose and Send the Email**

- Add a Gmail node.
- Set it to "Send Email" or "Create Draft" if you want to review it first.
- Use the extracted email address and body content.

**Confirmation Message**

- Send a confirmation back to your phone using Twilio.

**C. Get Calendar**

1. **Determine the Date Range** (Similar to fetching emails).
2. **Fetch Events from Google Calendar**

- Add a Google Calendar node.
- Set it to "Get Events" with the determined date range.

**Send Event Summaries via Twilio**

- Compose a message with the event details and send it to your phone.

**D. Create Task**

**Extract Task Details**

Copy`Extract the task details from the following message.  Message: {{Your Message Here}} Current Date: {{Current Date}}  Output: Task Name: [Name] Due Date: [Date]`

**Create Task in Notion**

- Add a Notion node.
- Set it to "Create Page" in your task database.
- Use the extracted task name and due date.

**Confirmation Message**

- Send a confirmation via Twilio.

**E. Create Meeting**

**Extract Meeting Details**

Copy`Extract the meeting details from the following message.  Message: {{Your Message Here}} Current Date: {{Current Date}}  Output: - Attendee Name: [Name] - Meeting Date: [Date] - Meeting Time: [Time] - Subject: [Subject]`

**Lookup Attendee Email** (Use Google Sheets).

**Create Event in Google Calendar**

- Add a Google Calendar node.
- Set it to "Create Event".
- Include the attendee's email and set up a Google Meet link if desired.

**Confirmation Message**

- Send a confirmation via Twilio.

**Step 5: Testing the Workflow**

Always test each action to ensure everything works smoothly.

**Example Test: Creating a Meeting**

- **Message Sent**: _"Can you schedule a meeting with Rahul next Thursday at 2 PM about the new project?"_

**Expected Outcome**:

- A new event is created in Google Calendar.
- Rahul receives an email invitation.
- You receive a confirmation via SMS.

**Personal Reflections**

Building this AI assistant was both challenging and rewarding. It took me about an hour to set up the initial version, but I can see endless possibilities for expansion. The key is to think about the tasks that consume your time and see how you can automate them.

One thing I learned is the importance of crafting precise prompts for OpenAI. The better the prompt, the more accurate the AI's responses. Also, integrating various tools like Gmail, Google Sheets, and Notion was surprisingly straightforward with n8n.

**Tips and Tricks**

- **Use Clear Prompts**: When working with OpenAI, providing clear instructions and examples improves accuracy.
- **Test Frequently**: After setting up each node, test it to catch any issues early.
- **Keep Security in Mind**: Make sure to secure your API keys and personal data.
- **Start Simple**: Begin with basic actions and gradually add complexity.

**Potential Enhancements**

- **Natural Language Understanding**: Improve the AI's ability to handle more complex language or ambiguous requests.
- **Error Handling**: Add nodes to handle exceptions or unrecognized commands gracefully.
- **Voice Commands**: Integrate with voice assistants beyond Siri, like Alexa or Google Assistant.
- **User Authentication**: Ensure that only authorized users can trigger certain actions.

I hope this guide inspires you to build your own AI assistant. Feel free to customize it to your needs, and don't hesitate to reach out if you have questions or want to share your creations.