
# Laboratory 09: The Cloud Automation Engineer

## Mission Overview

This laboratory activity focuses on cloud automation using Bash shell scripting, Linux file permissions, and Cron job scheduling. The goal is to create an automated backup script that compresses application data and schedules it to run every night at 2:00 AM.

## Objectives

- Understand the basics of Bash shell scripting.
- Create a script that automatically backs up application data.
- Use `chmod` to make a script executable.
- Configure a Cron job to schedule automated backups.
- Document the script and Cron configuration using Markdown.
- Complete the ninth laboratory activity in the Cloud Computing Portfolio.

## Commands Executed

| Command | Purpose |
|---|---|
| `mkdir app-data` | Creates the application data directory. |
| `echo "This is critical client data." > app-data/data.txt` | Creates a test file containing sample data. |
| `nano backup.sh` | Creates or edits the backup script. |
| `chmod +x backup.sh` | Makes the script executable. |
| `./backup.sh` | Executes the backup script. |
| `ls -l backups/` | Lists the generated backup files. |
| `crontab -l` | Displays the current Cron jobs. |
| `env EDITOR=nano crontab -e` | Opens the Cron table using Nano. |

## Skills Learned

- Writing and executing Bash scripts.
- Using variables in automation.
- Creating compressed backups with `tar`.
- Managing Linux file permissions.
- Scheduling recurring tasks using Cron.
- Documenting cloud automation procedures using Markdown.

## Screenshots

The following screenshots provide evidence of the completed tasks:

- `screenshots/script-execution.png` – Shows the backup script execution and generated backup file.
- `screenshots/cron-schedule.png` – Shows the installed Cron job schedule.
