For some reason, the udhcpd service may not start automatically. It is safe to run the following (see also `runhostapd` script)

```bash
sudo /etc/init.d/networking restart
sudo service hostapd stop
sudo service hostapd start
sudo service udhcpd stop
sudo service udhcpd start

ps -ef | grep hostapd
ps -ef | grep udhcpd
route -n
ifconfig
```
Reference: http://elinux.org/RPI-Wireless-Hotspot

Wifi adapter: TP-LINK TL-WN722N

Note: Change the ssid and wpa_passphrase in `/etc/hostapd/hostapd.conf`.

* hostapd
```bash
   /etc/hostapd/hostapd.conf
   /etc/default/hostapd
```

* udhcpd
```bash
   /etc/udhcpd.conf
   /etc/default/udhcpd
```

* interfaces
```bash
   /etc/network/interfaces
```
