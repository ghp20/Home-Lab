# npm-stack

> Nginx Proxy Manager — reverse proxy with Let's Encrypt SSL automation

**Status:** 🟢 Active | **Portainer ID:** 146 | **Category:** 🔒 Networking & VPN

---

## 📖 Overview

Nginx Proxy Manager — reverse proxy with Let's Encrypt SSL automation.

This stack is part of the [🔒 Networking & VPN](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`npm`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${STORAGE_ROOT}/data:/data
${STORAGE_ROOT}/certs:/etc/letsencrypt
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
