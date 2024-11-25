# Home

Subhra Das Gupta edited this page on Oct 12, 2022 · [3 revisions](https://github.com/subhra74/xdm/wiki/Home/_history)

# Frequently asked questions

[](https://github.com/subhra74/xdm/wiki#frequently-asked-questions)

- ### How do I increase the volume of the movie or songs which I downloaded?
    
    [](https://github.com/subhra74/xdm/wiki#how-do-i-increase-the-volume-of-the-movie-or-songs-which-i-downloaded)
    

Select that download, right click and select ‘Convert’. Video converter will open. Now click on boost button to increase volume. At select target format and click convert.

- ### How can I convert the downloaded movie for my mobile phone?
    
    [](https://github.com/subhra74/xdm/wiki#how-can-i-convert-the-downloaded-movie-for-my-mobile-phone)
    

XDM has built in video converter which supports numerous devices and file formats. Right click on the downloads and select ‘Convert’. Select the target format/device and click convert.

- ### XDM does not capture download, How to fix it?
    
    [](https://github.com/subhra74/xdm/wiki#xdm-does-not-capture-download-how-to-fix-it)
    

First check if addon for your browser is installed. If not then install addon from XDM Menu->Tools->Browser Monitoring page. If addon is already installed, then probably the file type is not included in supported files list. You can add it from XDM Menu->Tools->Browser Monitoring and add the file extension under ‘XDM will automatically take over downloads from browser for below file types’ For example if DMG files are not being automatically downloaded by XDM, simply add this extension to supported file list as mentioned above. Please always check you are using the latest version of XDM, from XDM Menu->Help->Check for update. If XDM still does not downloads the file, please post the issue in: [https://github.com/subhra74/xdm/issues/](https://github.com/subhra74/xdm/issues/)

- ### XDM does not show ‘DOWNLOAD VIDEO’ option while playing video in browser, How to fix it?
    
    [](https://github.com/subhra74/xdm/wiki#xdm-does-not-show-download-video-option-while-playing-video-in-browser-how-to-fix-it)
    

First check if addon for your browser is installed. If not then install addon from XDM Menu->Tools->Browser Monitoring page. It could also be possible that video size is too small and XDM is ignoring the video. To make this work just goto XDM Menu->Tools->Browser monitoring and lower the value in ‘Download video larger than’ dropdown. Alternatively you can copy the address of the web page containing the video, goto XDM Menu->File->Download video, and paste the address. XDM will parse and download the video. If problem still persists then, please post the issue in: [https://github.com/subhra74/xdm/issues/](https://github.com/subhra74/xdm/issues/) Also with newer version of XDM video will appear in browser window ![](https://raw.githubusercontent.com/subhra74/snowflake-screenshots/master/Youtube.png)

- ### I am getting error saying ‘Failed to append/convert file parts, please check if the drive is full or write protected’, Why?
    
    [](https://github.com/subhra74/xdm/wiki#i-am-getting-error-saying-failed-to-appendconvert-file-parts-please-check-if-the-drive-is-full-or-write-protected-why)
    

You are using an older version of XDM or the video is encrypted and is not supported by XDM. If problem appears with all websites, please post the issue in: [https://github.com/subhra74/xdm/issues/](https://github.com/subhra74/xdm/issues/).

- ### XDM is incorrectly taking over downloads which I don't want it to takeover, how to stop this?
    
    [](https://github.com/subhra74/xdm/wiki#xdm-is-incorrectly-taking-over-downloads-which-i-dont-want-it-to-takeover-how-to-stop-this)
    

When the ‘NEW DOWNLOAD’ window appears, click on MORE.. button and select ‘Do not capture download from this address’. Alternatively if you want XDM to not to capture certain file type, like PDF, simply remove the file from supported files list. Goto XDM Menu->Tools->Browser monitoring and remove the file type from ‘XDM will automatically take over downloads from browser for below file types’ list. ![](https://user-images.githubusercontent.com/8403090/86363097-a3e3ce80-bc76-11ea-9f9e-c24af431c0a5.png)

- ### While playing video, XDM does not show different formats in ‘DOWNLOAD VIDEO’ popup, how to get all the formats?
    
    [](https://github.com/subhra74/xdm/wiki#while-playing-video-xdm-does-not-show-different-formats-in-download-video-popup-how-to-get-all-the-formats)
    

Select a different format in the video player of your browser, XDM will automatically include this format in ‘DOWNLOAD VIDEO’ panel. Alternatively copy the address of the web page containing the video and paste in ‘Download video’ dialog from, XDM Menu->File->Download video.

- ### How to increase download speed of XDM?
    
    [](https://github.com/subhra74/xdm/wiki#how-to-increase-download-speed-of-xdm)
    

You can optimize network settings of XDM, from XDM menu->Tools->Network optimization and select you connection type.

- ### While resuming a download XDM says, download session is expired, what to do?
    
    [](https://github.com/subhra74/xdm/wiki#while-resuming-a-download-xdm-says-download-session-is-expired-what-to-do)
    

Select the download and click refresh link, and then click ‘Open containing web page’. If you are downloading a file, XDM will automatically pick up the new download link. If it was a streaming video, then select that same format from ‘DOWNLOAD VIDEO’ panel. If it was a video download from ‘Download video’ menu, then select the same format from the dialog box. If that option is not there, check ‘Advanced setting’ checkbox, open the web page where you found the download, copy the download link and paste the new download url. Don't forget to click ‘Save’ if you are manually pasting the link

- ### How can I download files 1 by 1?
    
    [](https://github.com/subhra74/xdm/wiki#how-can-i-download-files-1-by-1)
    

There are two options:

1. Set ‘Maximum simultaneous downloads’ to 1. Then keep adding the downloads. While 1 download is in progress, other downloads will wait.
2. Use a download queue. While adding the download, click ‘MORE…’ and select the queue. You can create new queues from XDM Menu->Tools->Options->Queue and scheduler.

###