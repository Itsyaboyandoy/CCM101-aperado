# ☁️ Cloud Automation Engineer

## 🎯 Mission Overview

Congratulations! Your ability to secure cloud environments has proven you are ready for the highest level of operations. You have been promoted to the Cloud Automation and DevOps Team at CloudNova Technologies.

Up until now, you have been acting as a traditional systems administrator—typing commands manually one by one. In large enterprise environments scaling to thousands of servers, manual administration is too slow and highly prone to human error. To survive at scale, you must learn to automate.

Using the KillerCoda Playground, you will step into the role of a Cloud Automation Engineer. You will learn the basics of Bash shell scripting, create an automated backup routine, assign executable permissions, and configure the Linux Cron scheduler to run your code autonomously.

Remember: **If you have to do a task more than twice in the cloud, you should automate it.**

## 🎯 Objectives

At the end of this laboratory activity, you should be able to:

- Understand the fundamental syntax of a Bash shell script, including variables and basic commands.
- Use a command-line text editor (nano) to write and save executable scripts.
- Modify Linux file permissions using the `chmod` command.
- Understand task scheduling and the syntax of a Linux crontab.
- Document automation code and Cron job configurations using Markdown.
- Complete the final chapter of your GitHub Cloud Computing Portfolio.

## 🛠️ Commands Executed

The following commands were used during the laboratory activity to create sample application data, write and execute the backup script, and configure the scheduled task.

| Command | Purpose |
|---|---|
| `mkdir -p app-data` | Creates the application data folder. |
| `echo "This is critical client data." > app-data/data.txt` | Creates a sample file containing test data. |
| `nano backup.sh` | Opens Nano to create or edit the Bash backup script. |
| `chmod +x backup.sh` | Gives the backup script executable permission. |
| `./backup.sh` | Executes the backup script manually. |
| `mkdir -p "$BACKUP_DIR"` | Creates the backup directory if it does not exist. |
| `tar -czf` | Compresses application data into a `.tar.gz` archive. |
| `ls -lh backups/` | Checks the generated backup files and their sizes. |
| `crontab -e` | Opens the Cron configuration for editing. |
| `crontab -l` | Displays the currently configured Cron jobs. |

## ⚙️ Backup Automation Implementation

For this activity, I created a Bash script named `backup.sh` to automate the backup process of the sample application data.

The script uses variables to identify the source and backup directories and generates a timestamp for each backup filename. It also checks whether the application data directory exists before proceeding.

The `tar` command compresses the application data into a `.tar.gz` archive, while the `mkdir -p` command ensures that the backup directory is available.

I also modified the file permissions using `chmod +x` so that the script could be executed directly from the terminal.

## ⏰ Cron Job Scheduling

Linux Cron was introduced to schedule the backup script automatically.

The intended schedule for this activity is every day at 2:00 AM using the following Cron expression:

```cron
0 2 * * * /bin/bash /root/CCM101-aperado/Laboratory-09-Cloud-Automation-Engineer/backup.sh
```

The five fields represent the minute, hour, day of the month, month, and day of the week.

The `crontab -l` command was used to inspect the current schedule, while `crontab -e` was used to configure the scheduled task.

## 💡 Skills Learned

- Writing and executing Bash shell scripts.
- Using variables to organize and manage script values.
- Creating compressed backups using the Linux `tar` command.
- Managing file and directory permissions using `chmod`.
- Creating directories and organizing backup files.
- Understanding Linux Cron scheduling and its five-field syntax.
- Verifying script execution and backup output through terminal commands.
- Documenting automation procedures using Markdown.
- Maintaining and completing a GitHub Cloud Computing Portfolio.

## 📁 Laboratory Files

The following files and folders are included in this laboratory activity:

| File or Folder | Description |
|---|---|
| `README.md` | Laboratory overview, objectives, commands, and skills learned. |
| `automation-research.md` | Research about Bash scripting, variables, and Cron jobs. |
| `backup-script-guide.md` | Instructions and explanation of the automated backup script. |
| `reflection.md` | Personal reflection about the laboratory activity. |
| `backup.sh` | Bash script used to automate application data backups. |
| `app-data/` | Contains the sample application data used for testing. |
| `backups/` | Stores the generated compressed backup archives. |
| `screenshots/` | Contains screenshots documenting the laboratory process. |

## 🏁 Conclusion

This laboratory activity helped me understand how automation can make system administration more efficient and reliable. By using Bash scripting, Linux file permissions, and Cron scheduling, I learned how repetitive tasks such as creating backups can be automated instead of being performed manually.

Through this hands-on experience in the KillerCoda environment, I improved my Linux command-line skills and gained a better understanding of how automation contributes to cloud operations and DevOps practices.

**Mission: Cloud Automation Engineer — Completed.**
