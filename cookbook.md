# Cookbook

## Analyzing websites

- [HWaddress: MAC address and OUI lookup](https://hwaddress.com/) - information about manufacturer by MAC address
- [WhoIs](https://who.is/) - track IP and/or domain names
- [RIPE DB](https://apps.db.ripe.net/db-web-ui/#/query) - track IP address

## Preparing a Kali linux Live USB bootable  

- Create the Kali linux 2018 USB persistence  
How to prepare the USB to run [Kali linux persistence mode](./kali-persistence/01_kali-persistence.md)

## Scanning Wi-Fi with Kali Linux

[source article](http://www.inzoolee.com/capture-wifi-air-packets-kali-linux-wifi-adapter/)
Kill possible interfering processes and put `wlan0` interface to the monitor mode. After it you can use WireShark to observe 802.11 packets.
```
airmon-ng check kill
airmon-ng start wlan0
```
Change channel of interface `wlan0mon`:
```
ifconfig wlan1mon down
iwconfig wlan1mon channel 1
ifconfig wlan1mon up
```
