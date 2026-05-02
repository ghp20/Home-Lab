# paperlesngx-stack

> Document management — scan, OCR, tag, and search all your paperwork

**Status:** 🟢 Active | **Portainer ID:** 241 | **Category:** 📦 Productivity & Collaboration

---

## 📖 Overview

Document management — scan, OCR, tag, and search all your paperwork.

This stack is part of the [📦 Productivity & Collaboration](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`postgres`**
- **`redis`**
- **`tika`**
- **`gotenberg`**
- **`paperless`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${STORAGE_ROOT}/postgres/17/docker:/var/lib/postgresql/data
${STORAGE_ROOT}/data:/usr/src/paperless/data
${STORAGE_ROOT}/media:/usr/src/paperless/media
${STORAGE_ROOT}/consume:/usr/src/paperless/consume
${STORAGE_ROOT}/trash:/usr/src/paperless/trash
```

## ⚠️ Gotchas & Tips

⚠️ OCR processing is very CPU-intensive — large PDFs can take several minutes

⚠️ The consume folder must pre-exist or Paperless won't detect new documents

⚠️ Database performance is the bottleneck for search — use PostgreSQL, not SQLite

⚠️ Regular backups of both /usr/src/paperless/data and the database


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
