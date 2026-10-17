# Laboratory 09 – Cloud Automation Engineer

## Mission Overview

This laboratory activity focuses on automating application data backups using a Bash script and scheduling the script with Cron. The goal is to reduce manual work and help protect important client data.

## Objectives

- Understand the basic syntax of Bash scripts.
- Create and execute an automated backup script.
- Use Linux file permissions to allow script execution.
- Configure a Cron job to schedule backups every day at 2:00 AM.
- Document the automation process using Markdown.

## Commands Executed

| Command | Purpose |
|---|---|
| `mkdir app-data` | Creates the application data directory. |
| `echo "This is critical client data." > app-data/data.txt` | Creates a sample data file. |
| `nano backup.sh` | Opens the Nano text editor to create the script. |
| `chmod +x backup.sh` | Adds execute permission to the script. |
| `./backup.sh` | Runs the backup script. |
| `ls -l backups/` | Checks the generated backup archive. |
| `tar -tzf backups/*.tar.gz` | Lists the contents of the compressed backup. |
| `crontab -l` | Displays the installed Cron schedule. |
| `env EDITOR=nano crontab -e` | Opens the Cron configuration for editing. |

## Skills Learned

In this activity, I learned how to create and run a Bash script to automatically backup files. I created a folder containing a sample text file and used the 'tar' command to create a compressed backup. I also learned how to use 'chmod +x' to run the script and Cron to schedule the backup for every day at 2:00 a.m. Lastly, I verified that the backup file was created and contained the proper files. This activity helped me understand how automation simplifies work and protects critical data.
