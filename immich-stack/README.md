# immich-stack

> Self-hosted Google Photos alternative — photo/video backup with AI face recognition

**Status:** 🟢 Active | **Portainer ID:** 322 | **Category:** ⚡ Media & Entertainment

---

## 📖 Overview

Self-hosted Google Photos alternative — photo/video backup with AI face recognition.

This stack is part of the [⚡ Media & Entertainment](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`immich-server`**
- **`immich-machine-learning`**
- **`redis`**
- **`database`**
- **`immich-ml-cache`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${STORAGE_ROOT}/data:/data
${EXTERNAL_PATH}:/external
/etc/localtime:/etc/localtime:ro
immich-ml-cache:/mlcache
${STORAGE_ROOT}/postgres:/var/lib/postgresql
```

## ⚠️ Gotchas & Tips

⚠️ ML container needs GPU passthrough (NVIDIA CUDA or Intel QSV) for reasonable performance

⚠️ Initial library scan can take hours for large photo collections

⚠️ Face recognition accuracy depends on having sufficient training data

⚠️ Postgres must have pgvector extension — use the Immich-provided image


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
