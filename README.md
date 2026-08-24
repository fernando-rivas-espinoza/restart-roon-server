# Restart Roon Server
Sometimes Roon will display nothing except for `System Output` under settings > audio, not detecting output devices connected to the machine, without an option to restart the server in the UI. The commands in these files kill a Roon server running on a silicon Mac and open the app. This should allow you to start a new server in the app, where all of your zones and devices should then appear.
- The commands in install-command will make a copy of the refresh-roon script into `/opt/homebrew/bin` and give it execution permissions to make it globally executable.
- To restart your Roon server, type `refresh-roon` into the terminal.
  - If you're using the server in the app, it will attempt to reconnect for a few seconds before prompting you to switch. At this point, start a new server on your device.
  - If you don't have Roon open, this script will restart the server and open the app. You can then start a new server on your machine.
 
