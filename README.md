# Scheduling Cron Job In Linux
## Scheduling
Cron is a scheduling daemon that executes tasks at specified intervals. 
These tasks are called cron jobs and are mostly used to automate system maintenance or administration.

The cron jobs can be scheduled to run by a minute, hour, day of the
 month, month, day of the week, or any combination of these.

## Why use Cronjobs?
Here are the reasons for using Cronjobs in Linux:
* Helps OS to take a scheduled backup of log files or database.
* Delete old log files
* Archive and purge database tables
* Send out any notification email such as Newsletters, Password expiration email
* Regular clean-up of cached data
* Crontab is an ideal option to automate Unix jobs.
* It is used to automate system maintenance
### What is Crontab File:
Crontab (cron table) is a text file that specifies the schedule of cron jobs. 
There are two types of crontab files. 
The system-wide crontab files and individual user crontab files.

Users' crontab files are named according to the user’s name, and their location varies by operating systems. 
In Red Hat based distributions such as CentOS, crontab files are stored in the /var/spool/cron directory,
while on Debian and Ubuntu files are stored in the /var/spool/cron/crontabs directory.

Although you can edit the user crontab files manually, it is recommended to use the crontab command.
The /etc/crontab file and the scripts inside the /etc/cron.d directory are system-wide crontab files 
that can be edited only by the system administrators.

In most Linux distributions you can also put scripts inside the /etc/cron.{hourly,daily,weekly,monthly} directories, 
and the scripts will be executed every hour/day/week/month.

### Linux Crontab Command

	1. crontab -e 	Edit crontab file, or create one if it doesn’t already exist.
	2. crontab -l 	Display crontab file contents.
	3. crontab -r 	Remove your current crontab file.
	4. crontab -i 	Remove your current crontab file with a prompt before removal.
	5. crontab -u <username> - Edit other user crontab file. This option requires system administrator privileges.
![Capture](https://github.com/MdsifatHossain/Scheduling-Cron-Job-In-Linux/assets/105970897/aa1913d1-a688-4cae-82f2-3976cc4587a2)


