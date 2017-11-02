# rsnapshot configs for macOS sierra
You can use this as a starting point for setting up rsnapshot on your mac.
1. Edit the configs to fit your needs
2. execute
   `sudo mkdir -p /etc/rsnapshot; cp rsnapshot.conf rsnapshot.common.conf /etc/rsnapshot/; touch /etc/rsnapshot/rsnapshot.ignore`
3. run rsnapshot, for example:
   `rsnapshot -c /etc/rsnapshot/rsnapshot.conf sync` to create the backup
   `rsnapshot -c /etc/rsnapshot/rsnapshot.conf <interval>` to rotate the backup
