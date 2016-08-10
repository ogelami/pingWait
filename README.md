# pingWait
##### pingWait [-h] [-b] [--eternal] [-d N] [-v] [-t N] HOSTNAME

pingWait will send ping packets until target replies and will then terminate successfully.

positional arguments:
* HOSTNAME    Hostname or ip of the target host

optional arguments:
* -h, --help  show this help message and exit
* -b          Beep when found (default: False)
* --eternal   Will continue to ping (default: False)
* -d N        Sleep delay between pings in seconds (default: 5)
* -v          Verbose logging (default: False)
* -t N        Timeout for ping in seconds (default: 1)

Example :
 - ./pingWait 8.8.8.8 && echo "Server is now up."
 - ./pingWait 192.168.1.129 && echo "Server is now responding to ping" | nc -c 127.0.0.1 27016
 - ./pingWait 192.168.1.129 && echo "The server is now up and running" | mail -s "pingWait response" ogelami@gmail.com
 - ./pingWait 8.8.8.8 -b --eternal
