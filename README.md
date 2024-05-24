# crontab-nmap-automated-scanner
open your cli for kali or ubuntu
type "crontab -e"
type
0 2 * * * nmap -sS -T4 -Pn -p 1-65535 <target ip> -oN /path/to/output.log
press ctrl + 0 to save 
press enter
nb:


