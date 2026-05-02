# nebula-sync-stack

> Pi-hole sync — keep multiple Pi-hole instances in sync

**Status:** 🟢 Active | **Portainer ID:** 145 | **Category:** 📊 Dashboards & Utilities

---

## 📖 Overview

Pi-hole sync — keep multiple Pi-hole instances in sync.

This stack is part of the [📊 Dashboards & Utilities](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`orbital-sync`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
/path/to/data/apps_config/orbital-sync/data:/app/data
```

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
