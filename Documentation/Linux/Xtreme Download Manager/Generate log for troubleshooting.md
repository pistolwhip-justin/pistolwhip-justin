# Generate log for troubleshooting

Subhra Das Gupta edited this page on Jul 2, 2020 · [2 revisions](https://github.com/subhra74/xdm/wiki/Generate-log-for-troubleshooting/_history)

### Before doing these steps you should exit XDM if its already running. To exit XDM goto File->Exit from XDM window.

[](https://github.com/subhra74/xdm/wiki/Generate-log-for-troubleshooting#befor-doing-these-steps-you-should-exit-xdm-if-its-already-running-to-exit-xdm-goto-file-exit-from-xdm-window)

### After you are successfully able to start XDM with logging enabled, please reproduce the bug, so that errors appear in the log

[](https://github.com/subhra74/xdm/wiki/Generate-log-for-troubleshooting#after-you-are-successfully-able-to-start-xdm-with-logging-enabled-please-reproduce-the-bug-so-that-errors-appear-in-the-log)

If you are on Windows:

- Open command prompt from the start menu (type cmd to search in start menu)
- After command prompt opens, type C: and press Enter
- Then type cd "C:\Program Files (x86)\XDM" and press Enter.
- If it shows error like folder does not exists then type cd "C:\Programs Files\XDM"
- Now type "java-runtime\bin\java" -jar xdman.jar

On Linux:

- Open terminal
- type cd /opt/xdman
- jre/bin/java -jar xdman.jar

On Mac OS X:

- Open terminal from Applications->Utilities
- Type cd /Applications/xdm.app/Contents/MacOS/
- jre/bin/java -jar xdman.jar

###