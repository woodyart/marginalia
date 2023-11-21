# Setup local NTP server using systemd-timesyncd

## Server side

Edit `/etc/systemd/timesyncd.conf` file:

```
[Time]
NTP=ext1.ntp-srv.com ext2.ntp-srv.com
...
```

## Client side