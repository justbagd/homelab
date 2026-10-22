# Homelab Documentation

Last updated: YYYY-MM-DD

## 1. Overview

Short description of what this server is for.

- **Hostname:**
- **Location:** (apartment, shelf/desk, etc.)
- **IP address:** (static or DHCP reservation)
- **Primary use:**

## 2. Hardware

| Component | Details |
|-----------|---------|
| CPU | |
| RAM | |
| Boot drive | |
| Data drives | |
| Network | (1GbE, Wi-Fi, etc.) |
| Power | (UPS? model, runtime) |
| Other | |

**Physical notes:** power setup, cooling, anything to know before touching it.

## 3. Operating System

- **OS and version:**
- **Install date:**
- **Admin user:**
- **Notable packages or config:**

## 4. Services

| Service | Purpose | Port | Deployment | Config location | Data location | Access |
|---------|---------|------|------------|-----------------|---------------|--------|
| Example: Jellyfin | Media server | 8096 | Docker | `~/homelab/jellyfin/` | `/mnt/data/media` | LAN only |
| | | | | | | |

**Deployment files:** path to docker-compose files / repo URL:

**Startup order or dependencies:** (e.g., database must be up before app X)

## 5. Storage Layout

| Device | Mount point | Filesystem | Size | Contents |
|--------|-------------|------------|------|----------|
| | | | | |

Notes on RAID, snapshots, or free space thresholds to watch.

## 6. Backups

| What | Destination | Frequency | Method/tool | Retention |
|------|-------------|-----------|-------------|-----------|
| | | | | |

**Restore steps:**
1.
2.

**Last tested restore:** YYYY-MM-DD

## 7. Access and Security

- **SSH:** port, allowed users, key-only login? (which keys, where they are stored)
- **Remote access method:** (Tailscale, WireGuard, none)
- **Firewall rules:**
- **Exposed outside LAN:** (list services, or "nothing")
- **Reverse proxy / TLS:** (tool, domains, cert renewal method)
- **Credentials location:** (password manager name; never store secrets here)

## 8. Monitoring

- **How I know something is down:**
- **Alerts:** (tool, where they go)
- **Dashboards:** (URLs)
- **Log locations:**

## 9. Maintenance

### Update process
- **OS updates:**
- **Container/service updates:**
- **Things that have broken during updates:**

### Routine checks
- [ ] Disk space
- [ ] Backup status
- [ ] Pending updates
- [ ] Certificate expiry

## 10. Troubleshooting Runbook

| Symptom | Likely cause | Fix |
|---------|--------------|-----|
| | | |

**Useful commands:**

```bash
# service status
# logs
# restart
```

## 11. Rebuild Checklist

If the OS drive died today:

1. Reinstall OS (version, partition notes)
2. Restore config and compose files from (location)
3. Remount data drives
4. Bring services up in order
5. Restore from backup if needed
6. Verify each service in the table above

## 12. Safe Shutdown and Startup Order

1.
2.

## 13. Decision Notes

| Date | Decision | Why | Alternatives considered |
|------|----------|-----|-------------------------|
| | | | |

## 14. Changelog

| Date | Change | Notes |
|------|--------|-------|
| YYYY-MM-DD | Initial setup | |

## 15. TODO / Ideas

- [ ]
