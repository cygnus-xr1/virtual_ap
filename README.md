# virtual_ap
Setting up an access point with hostapd &amp; dnsmasq

Activate iface
```
sudo ifconfig wlxd85d4c8c2050 up 10.0.0.1
```

Start hostapd
```
sudo hostapd -d hostapd.conf
```

Start dnsmasq
```
sudo dnsmasq -d -C dnsmasq.conf
```

Enable forwarding
```
router.sh wlan0 wlxd85d4c8c2050
```
