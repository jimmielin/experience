# Common Networking Commands

## IP Address Resolution

* `/etc/hosts` is your friend.
* **Checking Name Resolution:** `getent hosts jimmielin.me` (glibc), `dig +short jimmielin.me`, `host`, `nslookup`, ...

## Firewalls

* `firewall-cmd` is your friend.
* Checking listening ports: `netstat -lntp` (CentOS: part of `net-tools` package)

