[edit](https://github.com/2cld/bf/edit/master/docs/README.md)
# Network Map

| External Service             | type | description | location    |
|------------------------------|------|-------------|-------------|
|      24.149.22.11   : 32400  | 6.3 plex | [cfPlex](https://24.149.22.11:32400) | cf |
|      24.149.22.11   : 32500  | 6.6 plex | [cfDVR](https://24.149.22.11:32500)  | cf |
|      24.149.22.xx   : 32400  | 6.3 plex | [bfPlex](https://24.149.22.11:32400)  | bf |
|      24.216.208.251 : 32400  | 0.6 plex | [slPlex](https://24.216.208.251:32400) | sl |
|      24.216.208.251 : 32500  | 0.9 plex | [slDVR](https://24.216.208.251:32500) | sl |
| test.christrees.com :  2020  | 6.2 ssh  | sg | cf |

## port forward

| External | Internal | IP | detail |
|-------|-------|---------------|---|
| 32400	| 32400	| 192.168.6.3 | [bfPlex](https://24.149.22.xx:32400) on bfPlex win10 | 


## Internal Service

| ns service admin    | type    | description | location    | mac |
|---------------------|---------|-------------|-------------|-----|
| [http://192.168.6.1/](http://192.168.6.1/) | ng | netgear?? ng on subnet | bf:ng | xx:77:46:F6:xx:xx |
| [http://192.168.6.2/](http://192.168.6.2/) | sg | disabled sg on subnet | bf:sg | xx:15:5D:00:C9:xx |
| [http://192.168.6.3/](http://192.168.6.3/) | cg | win10 laptop | bf:cg | xx:C3:7B:46:0C:xx |
| res | - | - | - | na |
| [http://192.168.6.4/](http://192.168.6.4/) | - | - | - | 00:00:00:00:00:04 |
| ns2 | - | - | backup | na |
| [http://192.168.6.5](http://192.168.6.5) | bf:ng2 | gw | - | xx:00:00:00:00:xx |
| [http://192.168.6.6](http://192.168.6.6) | bf:sg2 | nas | - | xx:11:32:08:c4:xx |
| [http://192.168.6.7](http://192.168.6.7) | bf:cg2 | proxmox 8.1.4 | - | 00:00:00:00:00:xx |
| [https://192.168.6.8/](https://192.168.6.8/) | - | - | - | xx:30:48:c7:82:xx |
| [https://192.168.6.9/](https://192.168.6.9/) |  - | - | - | xx:30:48:c7:82:xx |
| [http://192.168.6.10:5000/ nsadmin](http://192.168.6.10:5000/)  - | - | - | xx:30:48:c7:82:xx |
| Plex | - | - | - | na |
| [https://192.168.6.3:32400/ local](https://192.168.6.3:32400/) | plex | [bfPlex remote](https://24.149.22.11:32400) | cf:cg on cfPlex i7 win10 | xx:C3:7B:46:0C:xx |
| [http://192.168.6.11/](http://192.168.6.11/) | tuner | [HDHR-1080AD03](http://192.168.6.11/) | cf:tvswitch | 00:18:dd:08:0a:d0 |
| [http://192.168.6.12/](http://192.168.6.12/) | tv | FireTVMain | cf:wifi | 48:43:dd:74:f1:72	|
| [http://192.168.6.13/](http://192.168.6.13/) | tv | FireTVcat | cf:wifi | a4:08:01:60:57:35	|
|---------------------|---------|-------------|-------------|-----|
| Workstations | - | - | - | na |
| [http://192.168.6.30/](http://192.168.6.30/) | ws | -- | win10 core duo | xx:d9:f5:c8:c7:xx	|
| other | - | - | - | na |
| [http://192.168.6.40/](http://192.168.6.40/) | wifi | cellphone | pixel-6a | 88:54:1f:3a:77:03	|
| Security Cameras |---------|------|-------------|--|
| [http://192.168.6.161](http://192.168.6.161) | macDHCP | zmodo | camera web | - |
| [http://192.168.6.162](http://192.168.6.162) | macDHCP | zmodo | camera web | - |
| [http://192.168.6.163](http://192.168.6.163) | macDHCP | zmodo | camera web | - |
| [http://192.168.6.164](http://192.168.6.164) | macDHCP | zmodo | camera web | - |
| [http://192.168.6.165](http://192.168.6.165) | macDHCP | [zmodo remote](https://user.zmodo.com/#/home) | zmodo hub | - |


| Service admin link | description |
|---|---|
| [ng.cfu.net - 854G-1 - http://192.168.6.1/](http://192.168.6.1/) | cfu pop router |
| [status_device table](http://192.168.6.1/#/html/status/status_devicetable.html) | MAC Devices |
| [dhcp reservation](http://192.168.6.1/#/html/advanced/ip/advanced_ip_dhcpreservation.html) | DHCP Reservations |
| [port forwarding](http://192.168.6.1/#/html/advanced/security/advanced_security_advancedportforwarding.html) | Port Forwarding |
| [dmz hosting](http://192.168.6.1/#/html/advanced/security/advanced_security_dmzhosting.html) | DMZ |
| [Firewall Rules](http://192.168.6.1/#/html/advanced/security/advanced_security_firewallsettings.html) | Firewall Rules |
| tbd | tbd |

- DHCP 192.168.0.100-199
- DNS 8.8.8.8
- GW 192.168.0.1 255.255.255.0
- SSID: TP-LINK_24 (18-A6-F7-31-9C-06)
- SSID: TP-LINK_9C05_5G (18-A6-F7-31-9C-05)
- WAN
```
18-A6-F7-31-9C-07
IP Address:	24.216.208.251	Dynamic IP
Subnet Mask:	255.255.248.0	 
Default Gateway:	24.216.208.1	  
DNS Server:	71.10.216.1 , 71.10.216.2
```

## Coax

| Coax name  | source   | destination | locations |
| ---------- |----------|-------------|-----------|
| cable feed | fiber box | spl01    | box to spl01 |
| LivingRoom feed | spl01p2 | tv | lr |
| LivingRoom feed | spl01p3 | none | lr |
| Bedroom feed | spl01p4 | tv | br |
| basement feed | spl01p5 | tv | bm |

# Reference Docs
- sl network based on [https://netstack.org/](https://netstack.org/) sl.lan model [https://netstack.org/docs/lan/](https://netstack.org/docs/lan/)
  - ng.sl.lan network gateway [https://netstack.org/docs/lan/network/tp-link/](https://netstack.org/docs/lan/network/tp-link/)
  - sg.sl.lan storage gateway [https://netstack.org/docs/lan/storage/freenas/](https://netstack.org/docs/lan/storage/freenas/)
  - cg.sl.lan compute gateway [https://netstack.org/docs/lan/compute/proxmox/nswin11vm](https://netstack.org/docs/lan/compute/proxmox/nswin11vm)

