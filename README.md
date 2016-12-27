# Conference firewall

Setup a firewall on a linux system that blocks all incoming requests,
except those as a response on connections initiated by you.

This script uses the iptables firewall of the linux kernel.

## Setup

Copy, unzip or clone the repo into a folder and go to that folder :

    git clone https://github.com/ruleant/firewall.git
    cd firewall

## Start the firewall

    # ./firewall-load

## Reset the firewall

    # ./firewall-reset

## FAQ

1. I get a 'iptables-restore: not found' error

   Run this script as a priviliged user (root, or use sudo), or check if the iptables package is installed on your system.

## Improvements

Comments, suggestions and improvements are welcome in the issue tracker on Github : https://github.com/ruleant/firewall

## License

MIT (see LICENSE file)
