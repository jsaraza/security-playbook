Commands:

- verify target lists/hostnames (list scan)
    nmap -sL 192.168.0.1/24

- identify live hosts (ping scan)
    -sn

-sT	TCP connect scan – complete three-way handshake
-sS	TCP SYN – only first step of the three-way handshake
-sU	UDP scan
-F	Fast mode – scans the 100 most common ports
-p[range]	Specifies a range of port numbers – -p- scans all the ports



-O	OS detection
-sV	Service and version detection
-A	OS detection, version detection, and other additions
-Pn	Scan hosts that appear to be down

TIMING

Timing	Total Duration
T0 (paranoid)	9.8 hours
T1 (sneaky)	27.53 minutes
T2 (polite)	40.56 seconds
T3 (normal)	0.15 seconds
T4 (aggressive)	0.13 seconds



Option	Explanation
-T<0-5>	Timing template – paranoid (0), sneaky (1), polite (2), normal (3), aggressive (4), and insane (5)
--min-parallelism <numprobes> and --max-parallelism <numprobes>	Minimum and maximum number of parallel probes
--min-rate <number> and --max-rate <number>	Minimum and maximum rate (packets/second)
--host-timeout	Maximum amount of time to wait for a target host



SAVING SCAN REPORT
-oN <filename> - Normal output
-oX <filename> - XML output
-oG <filename> - grep-able output (useful for grep and awk)
-oA <basename> - Output in all major formats

-d ~ enable debugging
