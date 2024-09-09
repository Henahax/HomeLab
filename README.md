# HomeLab

## 🍗 HenahaxServer

- Hardware
  - Intel N100
  - external hard drive enclosure, fast usb connection
  - https://www.amazon.de/AIOPCWA-Support-Storage-2-5GbE-Computer/dp/B0D5LCLQL6
- OS: ProxMox
- VMs
  - 🛜 Router
    - OS: PfSense / OPNSense
  - 🐋 Docker
    - OS: Debian / Ubuntu
    - Containers
      - Portainer
      - Reverse Proxy: Nginx Proxy Manager / træfik
      - ...
  - 🏠 Home
    - OS: Home Assistant
  - 🖫 NAS
    - OS: OpenMediaVault / Unraid / TrueNAS
    - Files
      - Document Archive
      - Media
      - Backups

### Notes

- DNS, VPN, Reverse Proxy potentially on Router VM
