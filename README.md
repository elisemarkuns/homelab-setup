# Elise's Homelab Setup
### 🚀 Overview
This repository contains my personal home infrastructure as code. Instead of installing services directly on the OS, I run them as isolated containers for easy management, updates, and portability.

### 📦 Services Included
#### Core-Stack
| Service |	Function |
|---------|----------|
| [Portainer](https://github.com/portainer/portainer) | Docker GUI Management |
| [Traefik](https://github.com/traefik/traefik) | Reverse Proxy |
| [Homepage](https://github.com/gethomepage/homepage) | Homepage to access services from one place |
| [UptimeKuma](https://github.com/louislam/uptime-kuma) | WebGUI for monitoring service uptime and sending notifications on change |
| [socket-proxy](https://github.com/wollomatic/socket-proxy) | Allows containers to communicate with docker socket securely |
| [ddns-updater](https://github.com/qdm12/ddns-updater) | Dynamically update DNS for your domain |
| [wg-easy](https://github.com/wg-easy/wg-easy) | WebGUI for generating Wireguard config |
| [dockergc](https://github.com/clockworksoul/docker-gc-cron) | Docker garbage collection |
| [deunhealth](https://github.com/qdm12/deunhealth) | Automatically restart unhealthy services |

#### Media-Stack
| Service |	Function |
|---------|----------|
| [Jellyfin](https://github.com/jellyfin/jellyfin) | Media server |
| [Prowlarr](https://github.com/Prowlarr/Prowlarr) | Configure your indexers all in one place |
| [Radarr](https://github.com/Radarr/Radarr) | Radarr is a movie collection manager for Usenet and BitTorrent users. |
| [Sonarr](https://github.com/Sonarr/Sonarr) | Sonarr is a PVR (for TV shows etc) for Usenet and BitTorrent users. |
| [Lidarr](https://github.com/Lidarr/Lidarr) | Lidarr is a music collection manager for Usenet and BitTorrent users. |
| [FlareSolverr](https://github.com/FlareSolverr/FlareSolverr) | FlareSolverr is a proxy server to bypass Cloudflare and DDoS-GUARD protection. |
| [Tdarr](https://github.com/HaveAGitGat/Tdarr) | Automatic transcoding of video files (I'm running my whole stack on a gaming laptop from 2013 through proxmox, so I couldn't get HW acceleration working, but YMMV. |


### ⚠️ Disclaimer
This is for personal or educational use only.

When I first started setting this up, I knew nothing about docker and I was learning by following tutorials and it took me a lot of time and effort to troubleshoot some of the issues. As I kept adding more services and doing more troubleshooting, I started understanding more about what each setting is for, so some of the yml files are more janky than others. Once I was satisfied with the stack's functionally, I haven't really touched the code, as there was no need for my personal use. I might clean it up someday when I don't have a dozen other things to do, but until then consider this project as-is.
