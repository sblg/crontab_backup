## crontab_backup
##The software utility cron is a time-based job scheduler in Unix-like computer operating systems. 

crontab -l #see a list of the current users cron jobs
crontab -e #edit crontab

##export your favourite editor, or you are directed to your default editor otherwise
export EDITOR=/usr/bin/nano

##code
##zip your folder every monday at 00. For more info regarding time: https://en.wikipedia.org/wiki/Cron.
# ┌───────────── minute (0 - 59)
# │ ┌───────────── hour (0 - 23)
# │ │ ┌───────────── day of month (1 - 31)
# │ │ │ ┌───────────── month (1 - 12)
# │ │ │ │ ┌───────────── day of week (0 - 6) (Sunday to Saturday;
# │ │ │ │ │                                       7 is also Sunday on some systems)
# │ │ │ │ │
# │ │ │ │ │
# * * * * *  command_to_execute

0 0 * * 1 tar czf <name_folder>.tar.gz <folder_location>


