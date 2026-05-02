# vaultwarden-stack

> Self-hosted Bitwarden — secure password manager for all devices

**Status:** 🟢 Active | **Portainer ID:** 50 | **Category:** 📦 Productivity & Collaboration

---

## 📖 Overview

Self-hosted Bitwarden — secure password manager for all devices.

This stack is part of the [📦 Productivity & Collaboration](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`db`**
- **`vaultwarden`**
- **`vaultwarden-net`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${STORAGE_ROOT}/postgres:/var/lib/postgresql/data
${STORAGE_ROOT}/data:/data
```

## ⚠️ Gotchas & Tips

⚠️ Without SMTP configured, users cannot recover/reset their master password

⚠️ Database backups are critical — vault data is irretrievable if corrupted

⚠️ Disable signups (SIGNUPS_ALLOWED=false) after creating user accounts

⚠️ WebSocket port must be exposed through reverse proxy for browser extension sync


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
