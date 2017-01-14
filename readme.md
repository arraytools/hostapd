```bash
sudo service hostapd start
sudo service udhcpd restart

ps -ef | grep hostapd
ps -ef | grep udhcpd

sudo service --status-all
```
Reference: http://elinux.org/RPI-Wireless-Hotspot

Wifi adapter: TP-LINK TL-WN722N

Note: Change the ssid and wpa_passphrase in `/etc/hostapd/hostapd.conf`.
