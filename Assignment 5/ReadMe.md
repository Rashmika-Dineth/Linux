# Assignment 5

### Make a script and add it to cron

- using crontab automation, let the script "print.sh" run every 12 hours, that is, twice a day

- Write the script "print.sh", that adds one line to file "diskspace.txt" reporting home directory size and date, example:
- - 3596 Jan 31 13:26:11 EET 2025
- let the script run minimum 6 times (there are at least 6 lines in file "discspace.txt" now)

- now write a command using awk-tool (manual) to find a line containing maximum size from "discspace.txt" and print it. Example output:
- - Max=3596, at Jan 31 13:26:11 EET 2025

1. First we need to identify the current size of the directory size. for this we can use

<tab><tab> du -s $HOME
