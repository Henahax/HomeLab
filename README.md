# HomeLab

## 🍗 HenahaxServer

- Hardware
  - Intel N100
  - external hard drive enclosure, fast usb connection
- OS: ProxMox
- VMs
  - 🛜 Router
    - OS: PfSense / OpenSense
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
