# HomeLab

## Server

- **IP-Address:** `x.x.x.1`
- **Hardware**
  - [Intel N100](https://www.amazon.de/AIOPCWA-Support-Storage-2-5GbE-Computer/dp/B0D5LCLQL6)
  - external hard drive enclosure, fast usb connection
- **OS:** [ProxMox](https://www.proxmox.com/)
- **VMs**
  - **🛜 Router**
    - IP-Address: `x.x.x.2`
    - OS: [pfSense](https://www.pfsense.org/) / [OPNsense](https://opnsense.org/)
  - **🐋 Docker**
    - IP-Address: `x.x.x.3`
    - OS: [debian](https://www.debian.org/index.de.html/) / [Ubuntu](https://ubuntu.com/)
    - Containers
      - Dynamic DNS: [CloudFlare DDNS](https://hub.docker.com/r/oznu/cloudflare-ddns/)
      - Container Management: [Portainer](https://www.portainer.io/) / [Dockge](https://dockge.kuma.pet/)
      - Reverse Proxy: [Nginx Proxy Manager](https://nginxproxymanager.com/) / [træfik](https://traefik.io/)
      - VPN Server: [WireGuard](https://www.wireguard.com/)
      - personal Websites
      - ...
  - **🖫 NAS**
    - IP-Address: `x.x.x.4`
    - OS: [OpenMediaVault](https://www.openmediavault.org/) / [Unraid](https://unraid.net/) / [TrueNAS](https://www.truenas.com/)
    - Files
      - Document Archive
      - Media
      - Backups
  - **🏠 Home**
    - IP-Address: `x.x.x.5`
    - OS: [Home Assistant](https://www.home-assistant.io/)

### Notes

- DynDNS, DNS, VPN, Reverse Proxy potentially on Router VM
