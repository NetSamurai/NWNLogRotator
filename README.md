# NWNLogRotator
Transforms and parses any Neverwinter Nights chat log into beautiful HTML. Written in C# .NET. NWNLogRotator is both Enhanced Edition and 1.69 compatible. <a href="http://htmlpreview.github.io/?https://github.com/notsigma/NWN-Log-Rotator/blob/master/output/NWNLogExample.html">Click here</a> for an example of a parsed log.

# Download
Latest version can be found <a href="https://github.com/notsigma/NWNLogRotator/releases/latest">here</a>.

# Screenshot
![Screenshot of NWNLogRotator would be here](https://raw.githubusercontent.com/notsigma/NWNLogRotator/master/Assets/Images/screenshot_nwnlr1.png)

# Automation (How it works)
While open, NWNLogRotator will process new logs automatically based on the status of whether Neverwinter Nights is running. Configure the directories to match with your Neverwinter Nights default log storage, and it will process them automatically.

# Configuration Examples
Important: Open Windows Explorer and enter %HOMEPATH%, and the last directory there is your _USER_.
  
| Configuration  | Example | Description |
| ------------- | ------------- | ------------- |
| Output Directory | C:\Users\\_USER_\Documents\Neverwinter Nights\logs\ | New logs stored in default Steam EE log directory |
| Output Directory | C:\Program Files (x86)\Neverwinter Nights\logs\ | New logs stored in default 1.69 log directory |
| Path to Log | C:\Users\\_USER_\Documents\Neverwinter Nights\logs\nwClientLog1.txt | Get log from Steam EE default log directory |
| Path to Log | C:\Program Files (x86)\Neverwinter Nights\logs\nwClientLog1.txt | Get log from 1.69 default log directory |
| Player Mode | True | NWNLogRotator will look for the player client |
| Server Mode | True | NWNLogRotator will look for server client |
| Server Name | Test | Server logs will be written to OutputDirectory\Test |
| Server Name Color | FFCC00 | The server name in the log appears yellow |
| Server Name Color | FF0000 | The server name in the log appears red |
| Custom Emotes | [],^ | [This will be an emote], ^This will be an emote^ |
| Filter Lines | foo,bar | Any line that has the word foo or bar will be removed |
| Auto Start | True,False | True will launch client on NWNLogRotator start |
| Auto Close | True,False | True will close client on Log creation |
| Theme | Dark, Light | Click on title, 'NWNLogRotator' to change Theme |

# Other Notes
1) This application may warn you that the publisher is not signed or verified, but if you click 'More Info' it will allow you to run anyways.
2) Make sure you save your configuration settings or some options may not do what you expected!
3) Make sure you have logging enabled if you cannot find a log file. The setting to enable logging is located in nwnplayer.ini as ClientEntireChatWindowLogging = 1 under [Game Options].