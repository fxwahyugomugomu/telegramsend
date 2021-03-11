# telegramsend
It is not a good practice to store your token in that place, but for now, it is ok. Also, you could limit actions your bot could do in the Channel only to send messages.

To run this script we should add permission

1. chmod +x telegramsend.sh
Now you can test it

2. ./telegramsend.sh "Test message"
In order to use this script from everywhere and type telegram-send instead ./telegramsend.sh add it to /usr/bin/ folder

3. sudo mv telegramsend.sh /usr/bin/telegramsend
Owner of all files in /usr/bin is root user. So let’s do the same with our script:

4. sudo chown root:root /usr/bin/telegramsend
Now you can test it

5. telegramsend "Test message"


Send notification on SSH login
All files with .sh extension in /etc/profile.d/ folder will be executed whenever a bash login shell is entered or the desktop session loads.

Let’s add a new script to send the notification.

1. nano login-notify.sh
Then move this script to /etc/profile.d/ folder
2. sudo mv login-notify.sh /etc/profile.d/login-notify.sh
Now re-login to your web server and check it works.
