# pingWait
Project written in python which will wait until target responds to a ping request and will then terminate.

usage: pingWait [-h] [-b] [--eternal] [-d N] [-v] [-t N] HOSTNAME

positional arguments:
  HOSTNAME    Hostname or ip of the target host.

optional arguments:
  -h, --help  show this help message and exit
  -b          Beep when found
  --eternal   Will continue to ping.
  -d N        Sleep delay between pings.
  -v          Verbose
  -t N        Ping timeout in seconds.
