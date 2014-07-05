Have cjdroute run as it's own user in it's own specific tunnel
=========================
Ultimately these are some pretty trivial tweaks to make cjdns run such that User=cjdns using a tunnel named cjdroute0. The
rc.local here sets up the tunnel automatically when you boot, and the cjdns.service file has User=cjdns added under [service].
Of course you have to do 'sudo adduser cjdns' and set cjdroute.conf to run as cjdns. Figuring out how to automatically 
configure that for my whole distro project.

