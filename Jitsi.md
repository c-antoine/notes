# Jitsi installation && configuration (~ ubuntu 18.04)

Full sudo
```bash
sudo -s
```

Restart all services
```bash
systemctl restart prosody jicofo jitsi-videobridge2 apache2
```
Install
```bash
sudo apt update
sudo apt install jitsi-meet
```

Open firewall with ufw
```bash
sudo ufw allow 80/tcp
sudo ufw allow 443/tcp
sudo ufw allow 4443/tcp
sudo ufw allow 10000/udp
sudo ufw allow 22/tcp
sudo ufw enable
```

Check ufw
```bash
sudo ufw status verbose
```

Check logs
```bash
cat /var/log/jitsi/jvb.log
cat /var/log/jitsi/jicofo.log
cat /var/log/prosody/prosody.log
cat /var/log/prosody/prosody.err
cat /var/log/apache2/access.log
cat /var/log/apache2/error.log
```

Reset all, more coffee and focus
```bash
sudo apt-get --purge remove jitsi-videobridge2 jitsi-meet jitsi-meet-prosody jitsi-meet-web jitsi-meet-web-config jicofo jitsi-videobridge
sudo rm /var/lib/dpkg/info rm jitsi-videobridge2.list
sudo rm /var/lib/dpkg/info rm jitsi-videobridge2.postrm
```
