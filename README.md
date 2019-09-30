# Edge Security

## Installation

### Requirements

#### software
   - [etcher](https://www.balena.io/etcher/) or dd
   - latest copy of [Hypriot](https://github.com/hypriot/image-builder-rpi/releases)
   - IDE or $EDITOR of choice for changing passwords in files located in src/*
   
#### hardware
   - [64Gb+ sdcard](https://www.amazon.com/dp/B073JYVKNX/)
   - [Raspberry Pi 4 2Gb](https://www.amazon.com/dp/B07TKFFCF1/) or better
   - network equipment (router, cables, isp uplink)
   
### Howto

1) [Burn hypriot to an sdcard](https://blog.hypriot.com/getting-started-with-docker-and-linux-on-the-raspberry-pi/)
2) Mount the sdcard
3) Copy user-data and docker-compose.yml to the boot partition
4) unmount and install into pi
5) connect networking and power
6) Once port 80, 443, and 9000 are available (netcat/telnet/nmap to test) visit https://edgesec.local/admin to configure the pi-hole
7) Visit https://edgesec.local:9000/ to review logs for debugging
