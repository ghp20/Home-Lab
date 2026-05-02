# arr-stack

> Complete *Arr stack — Prowlarr, Radarr, Sonarr, Bazarr, LazyLibrarian, Cleanuparr

**Status:** 🟢 Active | **Portainer ID:** 255 | **Category:** ⚡ Media & Entertainment

---

## 📖 Overview

Complete *Arr stack — Prowlarr, Radarr, Sonarr, Bazarr, LazyLibrarian, Cleanuparr.

This stack is part of the [⚡ Media & Entertainment](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`options`**
- **`arrnet`**
- **`prowlarr`**
- **`radarr`**
- **`sonarr`**
- **`bazarr`**
- **`lazylibrarian`**
- **`cleanuparr`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${APPS_CONFIG}/prowlarr/config:/config
${APPS_CONFIG}/radarr/config:/config
${MEDIA_ROOT}/movies-english:/movies-english
${MEDIA_ROOT}/movies-hindi:/movies-hindi
${DOWNLOAD_ROOT}:/downloadsq
${USENET_ROOT}:/downloads
${APPS_CONFIG}/sonarr/config:/config
${DOWNLOAD_ROOT}:/downloadsq
${USENET_ROOT}:/downloads
${MEDIA_ROOT}/Tv:/tv
${APPS_CONFIG}/bazarr/config:/config
${MEDIA_ROOT}/movies-english:/movies-english
${MEDIA_ROOT}/movies-hindi:/movies-hindi
${MEDIA_ROOT}/Tv:/tv
${APPS_CONFIG}/lazylibrarian:/config
${DOWNLOAD_ROOT}/lazylibrarian:/downloadsq
${DOWNLOAD_ROOT}/complete:/complete
${MEDIA_ROOT}/Books/ebooks:/books/ebooks
${MEDIA_ROOT}/Books/audiobooks:/books/audiobooks
${APPS_CONFIG}/cleanuparr/config:/config
```

## ⚠️ Gotchas & Tips

⚠️ All services share a single network — ensure Prowlarr is configured first

⚠️ Download client (qBittorrent/SABnzbd) must be added individually to each *Arr app

⚠️ Path mappings in Radarr/Sonarr must match download client paths exactly

⚠️ Cleanuparr can delete wanted content if rules are too aggressive


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
