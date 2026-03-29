# Hotline Startup Scripts (1.1.1)
Startup scripts for the Hotline server - uses the "screen" command to manage a session. This also restarts the Hotline process if it crashes.

---
These start up the Hotline server at boot time with a "screen" process.

1. run: **./startupinstall**
2. Put **@reboot /home/hotlineuser/bin/hotline start** into your crontab

When you want to view the Hotline console, just enter "**screen -r**" in your shell.

To disconnect from the Hotline console just press **CTRL-A CTRL-D**. This will leave it running and you can reconnect to it again.

If you want to turn off the server respawning type "**touch /home/hotlineuser/HotlineFiles/nostart**". To reenable it type "**rm /home/hotlineuser/HotlineFiles/nostart**".

---
Note: If you don't already have the "screen" tool installed you will need to install it by "**sudo apt-get install screen**".
