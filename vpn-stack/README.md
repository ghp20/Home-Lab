# vpn-stack

> VPN-protected download stack — Gluetun + qBittorrent + SABnzbd + Bitmagnet

**Status:** 🟢 Active | **Portainer ID:** 258 | **Category:** 🔒 Networking & VPN

---

## 📖 Overview

VPN-protected download stack — Gluetun + qBittorrent + SABnzbd + Bitmagnet.

This stack is part of the [🔒 Networking & VPN](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`arrnet`**
- **`options`**
- **`gluetun`**
- **`qbittorrent`**
- **`sabnzbd`**
- **`postgres-bitmagnet`**
- **`bitmagnet-process`**
- **`bitmagnet-worker`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${APPS_CONFIG}/gluetun:/gluetun
${APPS_CONFIG}/qbittorrent/config:/config
${DOWNLOADS_ROOT}:/downloadsq
${APPS_CONFIG}/sabnzbd/config:/config
${USENET_ROOT}:/downloads
${APPS_CONFIG}/bitmagnet/postgres:/var/lib/postgresql/data
${APPS_CONFIG}/bitmagnet/config:/config
${APPS_CONFIG}/bitmagnet/data:/data
${APPS_CONFIG}/bitmagnet/config:/config
${APPS_CONFIG}/bitmagnet/data:/data
```

## ⚠️ Gotchas & Tips

⚠️ Gluetun must start and connect to VPN before other services initialize

⚠️ Not all VPN providers support port forwarding — check before subscribing

⚠️ Bitmagnet database grows rapidly — monitor disk space regularly

⚠️ WireGuard keys must be valid and not expired


## 🚀 Deployment

1. **Review** the `docker-compose.yaml` file and update all `changeme` placeholder values
2. **Adjust** volume paths to match your storage layout
3. **Configure** environment variables — see the compose file for all options
4. **Deploy** using Portainer or Docker Compose:

```bash
docker compose -f docker-compose.yaml up -d
```

5. **Verify** containers are running:

```bash
docker compose -f docker-compose.yaml ps
```

## 🔗 Related Stacks

See the [root README](../README.md) for the full stack index organized by category.

---

*📝 README maintained as part of the Home-Lab repository. Last updated: {datetime.now().strftime('%Y-%m-%d')}*
