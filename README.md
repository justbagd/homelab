# Homelab Documentation

Last updated: 2026-10-22

## 1. Overview

Short description of what this server is for.

- **Hostname:** triilionair
- **Location:** apartment
- **IP address:** 10.250.16.39
- **Primary use:** Self-Hosting

## 2. Hardware

| Component | Details |
|-----------|---------|
| CPU | Intel Core i5-10600T CPU @ 2.40GHz |
| RAM | 16GB |
| Boot drive | 256GB NVMe |
| Data drives | 512GB SSD|
| Network | |
| Power | |
| Other | |

**Physical notes:** power setup, cooling, anything to know before touching it.

## 3. Operating System

- **OS and version:** ZimaOS 1.8.0
- **Install date:** 
- **Admin user:** triilionair
- **Notable packages or config:**

## 4. Services

| Service | Purpose | Port | Deployment | Config location | Data location | Access |
|---------|---------|------|------------|-----------------|---------------|--------|
| Jellyfin | Media server | 8096:8096 | Docker | `/DATA/AppData/jellyfin` | `` | Reverse Proxy |
| Sonarr | Media Management | 8989:8989 | Docker | `/DATA/AppData/sonarr` | `` | LAN |
| Radarr | Media Management | 7878:7878 | Docker | `/DATA/AppData/radarr` | `` | LAN |
| Seer | Media Request | 5055:5055 | Docker | `/DATA/AppData/seer` | `` | LAN |
| Prowlarr | Media Indexer | 9696:9696 | Docker | `/DATA/AppData/prowlarr` | `` | LAN |
| Profilarr | Media Profiles | 6868:6868 | Docker | `/DATA/AppData/profilarr` | `` | LAN |
| qBittorrent | Torrent Downloader | 8080:8080 | Docker | `/DATA/AppData/qbittorrent` | `` | LAN |
| Qui | qbit GUI | 7476:7476 | Docker | `/DATA/AppData/qui` | `` | LAN |
| Flaresolverr | Cloudflare Solver| 8191:8191 | Docker | `/DATA/AppData/flaresolverr` | `` | LAN |
| Open-webui | ollama GUI | 3000:8080 | Docker | `/DATA/AppData/open-webui` | `` | LAN |
| Ollama | AI Models | 11434:11434 | Docker | `/DATA/AppData/ollama` | `` | LAN |
| Dozzle | Docker Logs | 8888:8080 | Docker | `/DATA/AppData/dozzle` | `` | LAN |
| Portainer | Docker Management | 8000:8000, 9000:9000, 9443:9443 | Docker | `/DATA/AppData/portainer` | `` | LAN |
| Homarr | Dashboard | 7575:7575 | Docker | `/DATA/AppData/homarr` | `` | LAN |
| Tailscale | Remote Access | | Docker | `/DATA/AppData/tailscale` | `` | LAN |
| Netbird | Reverse Proxy | | Docker | `/DATA/AppData/netbird` | `` | LAN |



**Deployment files:** path to docker-compose files / repo URL: 

**Startup order or dependencies:** (e.g., database must be up before app X)

## 5. Access and Security

- **Remote access method:** Tailscale
- **Firewall rules:**
- **Exposed outside LAN:** (list services, or "nothing")
- **Reverse proxy / TLS:** (tool, domains, cert renewal method)

## 6. Monitoring

- **How I know something is down:**
- **Alerts:** (tool, where they go)
- **Dashboards:** (URLs)
- **Log locations:** Dozzle

## 7. Rebuild Checklist

If the OS drive died today:

1. Reinstall OS (version, partition notes)
2. Restore config and compose files from (location)
3. Remount data drives
4. Bring services up in order
5. Restore from backup if needed
6. Verify each service in the table above

