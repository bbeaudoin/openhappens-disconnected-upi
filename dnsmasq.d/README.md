This directory contains two dnsmasq.d configuration files used in different parts of my lab.

#. dhcp.conf -- Physical host (router/gateway) for issuing IP addresses to managed switches
#. origin.conf -- Bastion server (VM) serving as a proxy to services located in the internet DMZ.

These aren't meant to be fully inclusive nor must they be exclusive of each other. The DNS services and DHCP services can be on the same host via dnsmasq eliminating the need for the isc-dhcpd process.
