# HomeLab

current system private

future system in planning:

## 🍗 HenahaxServer

- **IP:** `x.x.x.2`
- **OS:** [ProxMox](https://www.proxmox.com/)
- **Hardware**
  - Intel N100: [example](https://www.amazon.de/AIOPCWA-Support-Storage-2-5GbE-Computer/dp/B0D5LCLQL6)
  - external hard drive enclosure, fast usb connection
- **VMs**
  - **🛜 HenahaxRouter**
    - IP: `x.x.x.1`
    - OS: [pfSense](https://www.pfsense.org/) / [OPNsense](https://opnsense.org/)
  - **🐋 HenahaxDocker**
    - IP: `x.x.x.3`
    - OS: [debian](https://www.debian.org/index.de.html/) / [Ubuntu](https://ubuntu.com/)
    - Containers:
      - Dynamic DNS: [CloudFlare DDNS](https://hub.docker.com/r/oznu/cloudflare-ddns/)
      - Container Management: [Portainer](https://www.portainer.io/) / [Dockge](https://dockge.kuma.pet/)
      - Reverse Proxy: [Nginx Proxy Manager](https://nginxproxymanager.com/) / [træfik](https://traefik.io/)
      - VPN Server: [WireGuard](https://www.wireguard.com/)
      - Personal Websites: [Nginx](hhttps://nginx.org/)
      - ...
  - **🖫 HenahaxNAS**
    - IP: `x.x.x.4`
    - OS: [OpenMediaVault](https://www.openmediavault.org/) / [Unraid](https://unraid.net/) / [TrueNAS](https://www.truenas.com/)
    - Files:
      - Document Archive
      - Media
      - Backups
  - **🏠 HenahaxHome**
    - IP: `x.x.x.5`
    - OS: [Home Assistant](https://www.home-assistant.io/)

### Notes

- DynDNS, DNS, VPN, Reverse Proxy potentially on Router VM
