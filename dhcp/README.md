This is the config that got me into the most trouble. Essentially the option for routers needs to be set, otherwise things will go sideways after the first reboot. The bootstrap will still connect to port 6443/tcp and masters will get their configuration from port 23623/tcp but, on reboot, the masters will forget their assigned hostnames as the default interface will be set to loopback.