# Intro
Running this command can unban Bangladeshi IPs from the server.

Only works if you are using [CSF Firewall][1].

## Commands

``` bash
#!/bin/bash
cat /etc/csf/csf.deny | grep BD/Bangladesh
sed -i '/Bangladesh/d' /etc/csf/csf.deny
csf -r
```

[1]: https://configserver.com/configserver-security-and-firewall/
