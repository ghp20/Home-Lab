# trading-agent-ron-stack

> AI trading agent — automated stock/crypto trading strategies

**Status:** 🟢 Active | **Portainer ID:** 307 | **Category:** 💰 Finance

---

## 📖 Overview

AI trading agent — automated stock/crypto trading strategies.

This stack is part of the [💰 Finance](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`trading-agent-ron`**
- **`trading-postgres-ron`**
- **`trading-redis-ron`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${STORAGE_ROOT}/config/config.yaml:/app/config/config.yaml:ro
${STORAGE_ROOT}/config/.env:/app/config/.env:ro
${STORAGE_ROOT}/models:/app/models
${STORAGE_ROOT}/logs:/app/logs
${STORAGE_ROOT}/data:/app/data
${STORAGE_ROOT}/src/:/app/src/
${STORAGE_ROOT}/postgres:/var/lib/postgresql/data
${STORAGE_ROOT}/redis:/data
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
