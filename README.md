# crontab-nmap-automated-scanner
open your cli for kali or ubuntu
type "crontab -e"
type
0 2 * * * nmap -sS -T4 -Pn -p 1-65535 <target ip> -oN /path/to/output.log
press ctrl + 0 to save 
press enter
nb:
0 2 * * *: Scheduled the cron job to run daily at 2:00 AM.
nmap -sS -T4 -Pn -p 1-65535 <target_IP_or_range> -oN /path/to/output.log: Command to execute the Nmap scan with specific options:
-sS: SYN scan for port scanning.
-T4: Timing template for faster scanning.
-Pn: Skip host discovery (assume all hosts are up).
-p 1-65535: Scan all ports.
<target_IP_or_range>: Defined the target IP address or range for scanning.
-oN /path/to/output.log: Saved scan results to a log file.

