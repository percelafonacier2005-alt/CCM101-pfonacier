# Backup Script Guide


## Backup Script Code

The following Bash script creates a compressed backup of the `app-data` directory.

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies
SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## File Permissions

The command `chmod +x backup.sh` adds execute permission to the script. This allows Linux to run the script as a program using `./backup.sh`.

# Cron Job Configuration

The Cron expression used is:

```bash
0 2 * * * /root/backup.sh
```

This schedules the backup script to run every day at 2:00 AM, based on the system's time.

### Cron Field Explanation

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute zero |
| Hour | `2` | At 2 AM |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

## Backup Verification

The command `./backup.sh` runs the backup script. The command `ls -l backups/` checks the generated backup file, while `tar -tzf backups/*.tar.gz` lists the contents of the compressed archive.

The expected archive contains `app-data/` and `app-data/data.txt`.
