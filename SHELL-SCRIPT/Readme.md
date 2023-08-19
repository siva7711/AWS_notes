# SHELL COMMANDS

CAT    - open file read mode

VIM    - create a file in edit mode

df     - printing the disk space

free   - Describe the free memory details

nproc  - no of CPU details

top    - prints all information like running processes, stoped ones ...etc 

set -x - Debug mode breifing like echo statement

ps -ef -  List all running processes ( process entire process in full length)

ps -ef | grep "systemd"  ( only systemd processes)

ps -ef | grep systemd | awk -F" " '{print $2}' ( to pick only 2nd column)

grep   - pick the selected one out of full output

man <commannd>  - describe about the command

awk   - pick specfic coloumns from the output

set -e - exit the script when there is a error

set -o - exit if pipe fails

curl - retrives the information from internet even downloads

curl <logs path> | grep "ERROR"  - retrive the error logs

curl -x GET api.foo.com     - get the information provided by api.foo.com

wget  - only download and store in the file.

sudo find / -name <filename>  - gives the file path where all it exists

sudo su -   (sudo root previlege su (swith user) -(root)

kill -9 <processid>  - kill the process id

trap  (while killing the process some signal will reach to linux system, not only killing in other cases also) you can trap the signal.
       
trap "echo dont use ctrl+c" SIGINT^C

trap "rm -rf *" ^cSIGINT  -- remove every thing if some one uses ctrl+c while processing.

below is the reference for linux signals

https://faculty.cs.niu.edu/~hutchins/csci480/signals.htm


