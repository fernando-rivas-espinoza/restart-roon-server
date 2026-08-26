# Restart Roon Server
On MacOS, Roon will sometimes display nothing except for `System Output` under settings > audio, not detecting output devices connected to the machine with no option to restart the server in the UI. The `refresh-roon` script will kill the running Roon server process and restart the app. This should allow you to start a new server in the app, where all of your zones and devices should then appear.
- The `install-command` script will make a copy of the refresh-roon script into `/opt/homebrew/bin` and give it execution permissions so it can run in any directory in the terminal
    ```bash
    $ zsh install-command
    ```
    >Make sure you're in the same directory as the file
- To restart your Roon server and app, run the script from the terminal
  ```bash
  $ refresh-roon
  ```
  - If you have the app running, the server process will stop and the app wil restart automatically
  - If you don't have Roon open, this script will restart the server and open the app. You can then start a new server on your machine
 
