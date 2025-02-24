
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
  

2. **Create a Script to Backup All Your Work:**
   

3. **Read About Cron and Crontab to Automate the Backup Script:**
   - Cron is the system's main scheduler for running jobs or tasks unattended. A command called crontab allows the user to submit, edit, or delete entries to cron. A crontab file is a user file that holds the scheduling information.

   **Answer**
   
   ![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day05/image/task%203.png)   
   ![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day05/image/task%203-1.png) 

4. **Read About User Management:**
   - A user is an entity in a Linux operating system that can manipulate files and perform several other operations. Each user is assigned an ID that is unique within the system. IDs 0 to 999 are assigned to system users, and local user IDs start from 1000 onwards.
   - Create 2 users and display their usernames.

   **Answer**
   
   ![image](https://github.com/Bhavin213/90DaysOfDevOps/blob/master/2024/day05/image/task%204.png)

[LinkedIn](https://www.linkedin.com/in/bhavin-savaliya/).
