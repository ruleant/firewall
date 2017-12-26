# Conference firewall

Setup a firewall on a linux system that blocks all incoming requests,
except those as a response on connections initiated by you.

This script uses the linux kernel netfilter firewall and configures it with iptables.

## Setup

Copy, unzip or clone the repo into a folder and go to that folder :

    git clone https://github.com/ruleant/firewall.git
    cd firewall

## Enable the firewall

    $ sudo ./firewall-load

## Reset the firewall

    $ sudo ./firewall-reset

## Make it persistent

To make the firewall rules persistent after a reboot, install the `iptables-persitent` package (Ubuntu\Debian) :

    $ sudo apt-get install iptables-persistent

This will save the current firewall rules and load them again after a restart.

Saving the firewall rules again after you changed them :

    $ sudo netfilter-persistent save

More info on how to use `netfilter-persitent` can be found on the [manpage](http://manpages.org/netfilter-persistent/8).

## FAQ

1. I get a 'iptables-restore: not found' error

   Run this script as a priviliged user (root, or use sudo), or check if the iptables package is installed on your system.

## Improvements

Comments, suggestions and improvements are welcome in the issue tracker on Github : https://github.com/ruleant/firewall

## License

MIT (see LICENSE file)
