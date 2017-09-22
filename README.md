# ipalert
A simple bash script that will e-mail you if your external IP address changes. Tested in Ubuntu but should work on most debian systems. It uses mutt and cron. 

## Setup
It is highly recommended to setup a dedicated e-mail for this. Most people use Gmail so this guide will show you how to use Gmail to send such alerts. 

### Gmail Configuration
The following settings will allow you to send e-mails via Gmail by using the command line. In this case we're using Mutt
1. Create a gmail account: https://accounts.google.com/SignUp
2. Turn on 2 step verification: https://support.google.com/accounts/answer/185839?hl=en&ref_topic=7189195
3. Create an app specific password for ipalert: https://security.google.com/settings/security/apppasswords 
4. Make note of this app-specific password, you will need it later.

### Run bootstrap.sh
The included bootstrap script should work for Debian and will setup the following:
1. Install system package dependencies. 
2. Dedicated user for the script and associated files.

### Configure Mutt
Take a look at the muttrc.example file. You can choose to use this as the global configuration file, /etc/Muttrc (notice the case sensitivity) or install it under a specific user ~/.muttrc. If you are using Gmail, remember to use the application specific password you created in step 3 of gmail configuration. 




