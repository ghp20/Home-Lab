# firefly3-stack

> Personal finance manager — track expenses, budgets, and bank transactions

**Status:** 🔴 Inactive | **Portainer ID:** 42 | **Category:** 💰 Finance

---

## 📖 Overview

Personal finance manager — track expenses, budgets, and bank transactions.

This stack is part of the [💰 Finance](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`firefly-db`**
- **`firefly-iii`**
- **`firefly-importer`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${STORAGE_ROOT}/database:/var/lib/mysql
${STORAGE_ROOT}/uploads:/var/www/html/storage/upload
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
