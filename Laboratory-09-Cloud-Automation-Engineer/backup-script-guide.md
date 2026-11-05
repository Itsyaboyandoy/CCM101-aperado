# ⚙️ Backup Script Guide

## 1. Backup Script

The `backup.sh` script automates the process of creating a compressed backup of the `app-data` folder. It saves the generated archive inside the `backups` directory and uses a timestamp to give each backup a unique filename.

### Script Code

```bash
#!/bin/bash

# CloudNova Technologies - Automated Backup Script

SCRIPT_DIR="$(cd "$(dirname "$0")" && pwd)"
SOURCE_DIR="$SCRIPT_DIR/app-data"
BACKUP_DIR="$SCRIPT_DIR/backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

if [ ! -d "$SOURCE_DIR" ]; then
    echo "Error: Source directory does not exist."
    exit 1
fi

mkdir -p "$BACKUP_DIR"

tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" \
    -C "$SCRIPT_DIR" app-data

if [ $? -eq 0 ]; then
    echo "Backup completed successfully at $TIMESTAMP!"
    echo "Backup saved in: $BACKUP_DIR"
else
    echo "Backup failed!"
    exit 1
fi
```

### Script Explanation

| Command or Variable | Purpose |
|---|---|
| `#!/bin/bash` | Specifies Bash as the script interpreter. |
| `SCRIPT_DIR` | Gets the directory where the script is located. |
| `SOURCE_DIR` | Identifies the application data folder. |
| `BACKUP_DIR` | Identifies where backup files will be stored. |
| `TIMESTAMP` | Generates a date and time for the backup filename. |
| `mkdir -p` | Creates the backup directory if it does not exist. |
| `tar -czf` | Compresses the application data into a `.tar.gz` archive. |
| `exit 1` | Stops the script when an error occurs. |

## 2. File Permissions and Execution

Before running the script, it must have executable permission.

The following command gives the script permission to run:

```bash
chmod +x backup.sh
```

To execute the backup script:

```bash
./backup.sh
```

To check whether the backup was successfully created:

```bash
ls -lh backups/
```

This command displays the generated backup archive, including its filename and file size.

## 3. Cron Job Schedule

A Cron job allows the backup script to execute automatically at a scheduled time.

For this activity, the script is scheduled to run every day at 2:00 AM.

### Cron Expression

```cron
0 2 * * * /bin/bash /root/CCM101-aperado/Laboratory-09-Cloud-Automation-Engineer/backup.sh
```

### Cron Field Breakdown

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2:00 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

### Adding the Cron Job

Open the Cron editor:

```bash
crontab -e
```

Add the following line:

```cron
0 2 * * * /bin/bash /root/CCM101-aperado/Laboratory-09-Cloud-Automation-Engineer/backup.sh
```

Save the file, then verify the scheduled task:

```bash
crontab -l
```

The command displays the currently configured Cron jobs for the user.

## 4. Summary

The backup script automates the process of compressing application data into a timestamped archive. Executable permissions allow the script to run, while the Cron job schedules it to execute automatically every night at 2:00 AM.

Through this activity, I learned how Bash scripting and Cron scheduling can work together to make repetitive system administration tasks easier and more efficient.
