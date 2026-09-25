# nmap

## quick scans
nmap -sC -sV -oA scan 10.10.10.10
nmap -p- --min-rate 5000 -T4 10.10.10.10
nmap -sU --top-ports 50 10.10.10.10

## notes
- Always `-oA` so you don't rescan.
- Full port sweep first, service scan second.
- UDP is slow — top ports only unless you have a reason.
