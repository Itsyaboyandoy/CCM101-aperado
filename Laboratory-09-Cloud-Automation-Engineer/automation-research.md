# 🔎 The Language of Automation

## 1. Bash Script

A Bash script is a file that contains Linux commands that can run together automatically. Instead of typing commands one by one in the terminal, we can place them inside a script and execute them whenever needed.

The `#!/bin/bash` line at the beginning is called a shebang. It tells Linux to use Bash to run the script.

In this laboratory activity, I created a Bash script named `backup.sh` to automate the process of creating compressed backups of application data.

## 2. Variables

Variables are used to store values that can be reused throughout a script. They make scripts easier to understand, organize, and update.

For example, the variable `$BACKUP_DIR` stores the location of the folder where backup files will be saved. Instead of repeatedly typing the folder path, I can simply use the variable.

Other variables used in the backup script include:

- `SOURCE_DIR` – stores the location of the application data.
- `BACKUP_DIR` – stores the location of the backup folder.
- `TIMESTAMP` – stores the current date and time to give each backup a unique filename.

## 3. Cron Job

A Cron job is a scheduled task in Linux that automatically runs commands or scripts at a specific time. It is useful for automating repeated tasks without requiring someone to execute them manually.

Cron uses five time fields to determine when a task should run:

1. Minute
2. Hour
3. Day of the month
4. Month
5. Day of the week

For this activity, I used the following Cron expression:

```cron
0 2 * * * /bin/bash /root/CCM101-aperado/Laboratory-09-Cloud-Automation-Engineer/backup.sh
```

This schedules the backup script to run every day at 2:00 AM.

## 4. Importance of Automation in Cloud Computing

Automation is important in cloud computing because it helps administrators perform repetitive tasks efficiently and consistently. Tasks such as backups, system maintenance, and monitoring can be automated to reduce manual work and human errors.

However, automation scripts must be tested carefully. Incorrect commands or configurations may cause unexpected results or data loss.

Through this activity, I learned how Bash scripts, variables, and Cron jobs work together to automate a simple backup process in a Linux environment.
