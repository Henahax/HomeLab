# HomeLab

current system private

future system in planning:

## **🍗 `Server`**

- **IP:** `192.168.0.2`
- **OS:** [ProxMox](https://www.proxmox.com/)
- **Hardware**
  - **CPU**
    - Intel N305 / Intel N355 / Intel Core i3-14100
  - **Mainboard**
    - 2+ Ethernet
    - 2+ NVMe
    - 4+ SATA
  - **Storage**
    - 2 SSDs for OS, VMs
    - SSD for Storage
    - HDD for Backup
  - **Case**
    - µATX / ITX
    - 2+ 3.5" HDD
    - 2+ 2.5" SSD
- **Virtual Machines**
  - **🛜 `Router`**
    - IP: `192.168.0.3`
    - OS: [OPNsense](https://opnsense.org/) / [pfSense](https://www.pfsense.org/)
  - **🐋 `Services`**
    - IP: `192.168.4`
    - OS: [debian](https://www.debian.org/)
    - Containers:
      - **Admin**:
        - Container Management: [Portainer](https://www.portainer.io/) / [Dockge](https://dockge.kuma.pet/) / [Arcane](https://arcane.ofkm.dev/)
        - Dashboard: [Homarr](https://homarr.dev/)
        - Monitoring: [Uptime Kuma](https://uptime.kuma.pet/)
        - Monitoring Dashboard: [Grafana](https://grafana.com/)
        - Notifications: [ntfy](https://docs.ntfy.sh/)
      - **Network**:
        - Dynamic DNS: [CloudFlare DDNS](https://hub.docker.com/r/oznu/cloudflare-ddns)
        - Reverse Proxy: [Nginx Proxy Manager](https://nginxproxymanager.com/) / [træfik](https://traefik.io/)
        - VPN Server: [WireGuard](https://www.wireguard.com/) / [tailscale](https://tailscale.com/)
        - DNS Ad Blocking: [Pi-hole](https://pi-hole.net/)
      - **Private**:
        - Media System: [Jellyfin](https://jellyfin.org/)
        - Document Management: [Paperless-ngx](https://docs.paperless-ngx.com/)
      - **Public**:
        - Personal Websites: [Node.js](https://nodejs.org/) / [Deno](https://deno.com/)
        - Voice-Chat: [teamspeak](https://www.teamspeak.com/)
      - **Misc**:
        - Research contribution: [Folding@home](https://foldingathome.org/)
        - SSH tarpit: [Endlessh](https://github.com/skeeto/endlessh)
        - Large Langugage Models: ollama
        - hedgedoc
        - File hosting: [Nextcloud](https://nextcloud.com/)
        - Photo & video management: [immich](https://immich.app/)
        - n8n
  - **🖫 `Data`**
    - IP: `192.168.0.5`
    - OS: [TrueNAS SCALE](https://www.truenas.com/truenas-scale/)
    - manages ZFS
    - Files:
      - Document Archive
      - Media
      - Backups
  - **🏠 `Home`**
    - IP: `192.168.0.6`
    - OS: [Home Assistant](https://www.home-assistant.io/)

### Notes

- Network Containers potentially on Router VM
