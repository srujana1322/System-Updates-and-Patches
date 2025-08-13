Script:

#!/bin/bash
#Update package lists apt-get update
#Upgrade all packages apt-get
-y upgrade
#Distribute updates to multiple servers servers=("server1" "server2" "server3") for server in "${servers[@]}"; do	ssh root@$server 'apt-get update
&& apt-get -y upgrade' done
#Notify administrator
echo "System updates and patches applied." | mail -s "Update Notification" admin@mycomp.com


This script updates and upgrades the system's package lists and packages. It also distributes updates to multiple servers via SSH. The script concludes by notifying the system administrator that updates have been applied.
