# Homelab

|||
|-|-|
|*Name*|**`Server`**|
|*IP-Address*|**`192.168.2`**|
|*Operating system*|**[ProxMox](https://www.proxmox.com/)**|

## Hardware

|Category|Reqirements|Choices|
|-|-|-|
|CPU|...|Intel N305 / Intel N355 / Intel Core i3-14100|
|Mainboard|2+ Ethernet||
||2+ NVMe||
||4+ SATA||
|Storage|||
|Case|||

## ZFS

## Virtual machines

### 🛜 Router

|||
|-|-|
|*Name*|**`Router`**|
|*IP-Address*|**`192.168.3`**|
|*Operating system*|**[OPNsense](https://opnsense.org/) / [pfSense](https://www.pfsense.org/)**|

### 💾 Data

|||
|-|-|
|*Name*|**`Data`**|
|*IP-Address*|**`192.168.5`**|
|*Operating system*|**[TrueNAS SCALE](https://www.truenas.com/truenas-scale/)**|
|*Software*||

#### "Volumes"

|Name|Description|
|-|-|
|Documents||
|Media||
|Volumes|persistent volumes of container services|

### 🐋 Services

|||
|-|-|
|*Name*|**`Services`**|
|*IP-Address*|**`192.168.4`**|
|*Operating system*|**[Debian](https://www.debian.org/)**|
|*Software*|**Docker**|

#### Containers

|Category|Description|Services|
|-|-|-|
|**Admin**|Container management|[Portainer](https://www.portainer.io/) / [Dockge](https://dockge.kuma.pet/) / [Arcane](https://arcane.ofkm.dev/)|
||Dashboard|[Homarr](https://homarr.dev/)|
||Monitoring|[Uptime Kuma](https://uptime.kuma.pet/)|
||Monitoring dashboard|[Grafana](https://grafana.com/)|
||Notifications|[ntfy](https://docs.ntfy.sh/)|
|**Network**|Dynamic DNS|[CloudFlare DDNS](https://hub.docker.com/r/oznu/cloudflare-ddns)|
||Reverse proxy|[Nginx Proxy Manager](https://nginxproxymanager.com/) / [træfik](https://traefik.io/)|
||VPN server|[WireGuard](https://www.wireguard.com/) / [tailscale](https://tailscale.com/)|
||DNS ad blocking|[Pi-hole](https://pi-hole.net/)|
|**Public**|Websites|[Node.js](https://nodejs.org/) / [Deno](https://deno.com/)|
||Voice chat|[teamspeak](https://www.teamspeak.com/)|
|**Private**|File hosting|[Nextcloud](https://nextcloud.com/)|
||Document management|[Paperless-ngx](https://docs.paperless-ngx.com/)|
||Photo & video management|[immich](https://immich.app/)|
||Media system|[Jellyfin](https://jellyfin.org/)|
||Personal notes|[Obsidian](https://obsidian.md/)|
||Collaborative notes|[HedgeDoc](https://hedgedoc.org/)|
||Large Langugage Model|[Ollama](https://ollama.com/)|
||Workflow automation|[n8n](https://n8n.io/)|
||Media automation|[Servarr](https://wiki.servarr.com/)|
|**Miscellaneous**|Research contribution|[Folding@home](https://foldingathome.org/)|
||SSH tarpit|[Endlessh](https://github.com/skeeto/endlessh)|

### 🏠 Home

|||
|-|-|
|*Name*|**`Home`**|
|*IP-Address*|**`192.168.6`**|
|*Operating system*|**[Home Assistant](https://www.home-assistant.io/)**|
|*Software*||
