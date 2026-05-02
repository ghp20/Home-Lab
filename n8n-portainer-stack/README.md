# n8n-portainer-stack

> Workflow automation — connect APIs, services, and trigger automations

**Status:** 🟢 Active | **Portainer ID:** 114 | **Category:** 🤖 AI & Development

---

## 📖 Overview

Workflow automation — connect APIs, services, and trigger automations.

This stack is part of the [🤖 AI & Development](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`n8n`**
- **`n8n-postgres`**
- **`default`**
- **`trading-net-ron`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${STORAGE_ROOT}/portainer-restore-test:/home/node/.n8n
${STORAGE_ROOT_BASE}/n8n/know_base:/home/node/.n8n-files
${STORAGE_ROOT}/postgres-data:/var/lib/postgresql/data
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
