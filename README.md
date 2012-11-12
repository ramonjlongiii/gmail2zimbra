gmail2zimbra
============

A handy script to automate email domain migrations from Gmail to Zimbra using imapsync.

# Script:       
gmail2zimbra.sh

# Version:      
v1.1

# Author:       
Ramon J. Long III <ramon@evolveinc.com>

# Credits:      
Modified from the script found on the official Zimbra Wiki.

# About:        
This script uses imapsync to transfer mailbox contents from
GMail / Google Apps to Zimbra.  Although this script has been
tested on Zimbra 8.0 Open Source, it should work on earlier
versions of ZCS.

# Usage:        
Make sure IMAP is enabled for each Google account in the
Account Preferences (it is turned off by default).  Change
host1 and host2 to the appropriate IPs of the source and
destination.  You can probably leave host1 as is unless
Google changes the IPs of imap.gmail.com.  You will have to make
sure your Zimbra accounts have already been provisioned.
Be sure to change the domain variable to the appropriate domain.

userlist.txt should be in the following format:

account1;password1
account2;password2

etc.  Do not include the domain in userlist.txt - this is
appended by the script.
