
# Day 5 Answers: Advanced Linux Shell Scripting for DevOps Engineers with User Management

### Tasks

1. **Create Directories Using Shell Script:**
#!/bin/bash
Directory_name=$1
Start_number=$2
End_number=$3

for ((i=Start_number; i<=End_number; i++))
do
        mkdir "${Directory_name}${i}"
done
echo "Directories are created succesfully"
  

2. **Create a Script to Backup All Your Work#!/bin/bash

#!/bin/bash
Destination_dir="/c/Users/Divya.Moykhede/git_tutorial/backupdir"
Timestamp=$(date +%Y%m%d_%H%M%S)   # Correct command substitution
Backup_file="backup_${Timestamp}.tar.gz"  # Use correct variable substitution
# Ensure the source directory exists and is valid
Source_dir="/c/Users/Divya.Moykhede/devopstest/backup_src"
# Make sure the destination directory exists
mkdir -p "$Destination_dir"
# Now, use the correct path for the tar command
tar czf "$Destination_dir/$Backup_file" -C /c/Users/Divya.Moykhede/devopstest backup_src
echo "Backup is created"
   
   

4. **Read About Cron and Crontab to Automate the Backup Script:**
   - Cron is the system's main scheduler for running jobs or tasks unattended. A command called crontab allows the user to submit, edit, or delete entries to cron. A crontab file is a user file that holds the scheduling information.
Lets create a crontab that schedules backup at 19th October 2pm
cron 00 14 19 10 * ./backup.sh

5. **Read About User Management:**
   - A user is an entity in a Linux operating system that can manipulate files and perform several other operations. Each user is assigned an ID that is unique within the system. IDs 0 to 999 are assigned to system users, and local user IDs start from 1000 onwards.
   - Create 2 users and display their usernames.
     #!/bin/bash
     sudo useradd user1
     sudo useradd user2
     cat /etc/passwd | grep -E "user1|user2"
     
     


