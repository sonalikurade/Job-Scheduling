# Job Scheduling
## What does Job Scheduling mean in Linux?

Job scheduling is a feature of Linux operating systems that allows users to schedule tasks to run automatically at specified times or intervals. This is done using a daemon called cron, which runs in the background and executes tasks based on entries in a configuration file called crontab. It’s help to get backup of files and directories.
## Two types of Job scheduling
1. at job
2. cron job scheduling

## There is few methods in Linux to Schedule Job

Crontab : which is short for cron table, is a file containing the schedule of various cron entries that should be run at specified times. Another way of describing crontab is as a utility that enables tasks to run automatically at regular intervals in the background by the cron daemon. A cron job is a command run by the cron daemon at regularly scheduled intervals. To submit a cron job, specify the crontab command with the -e flag. The crontab command invokes an editing session that allows you to create a crontab file. In a cron tab there are 5 expression denotes by using * .
Cronjob Syntax :

## There is Few option in Crontab Command

crontab -e : It is help to create or modify cronjobs
crontab -l : It use for list cronjobs
crontab -r : It use for remove all cronjobs
Example of crontab command in Linux: Suppose you want to schedule a job that will run the ls -l command every day at 2 PM, you can use the crontab command as follows. follow the bellow steps is run crontab -e command then open vi file editor tab as follow as


at : at is single time execution command. at command Queue a task in “/var/spool/at “ directory and execute when it’s schedule time. After execution the task is autoremove from queue
Example of at command : Suppose if you want to schedule a job at 2 PM, you can use the ‘at’ command as follows

atq — atq command use for list all jobs with job number scheduled by at command

atrm — this command use for remove jobs by using there job id. Use of atrm command as follows
atrm 10