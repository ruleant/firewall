# Conference firewall

Setup a firewall on a linux system that blocks all incoming requests,
except those as a response on connections initiated by you.

This script uses the iptables firewall of the linux kernel.

## Setup

Copy or clone the repo into a folder.

## Start the firewall

    cd /path/to/folder
    ./iptables-load

## Reset the firewall

    cd /path/to/folder
    ./iptables-reset

## FAQ

1. I get a 'iptables-restore: not found' error

   Run this script as a priviliged user (root, or use sudo), or check if the iptables package is installed on your system.

## Improvements

Comments, suggestions and improvements are welcome in the issue tracker on Github : https://github.com/ruleant/firewall

## License

MIT (see LICENSE file)
