# tdarr-stack

> Distributed media transcoding — automate codec/quality optimization

**Status:** 🔴 Inactive | **Portainer ID:** 201 | **Category:** ⚡ Media & Entertainment

---

## 📖 Overview

Distributed media transcoding — automate codec/quality optimization.

This stack is part of the [⚡ Media & Entertainment](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`tdarr`**
- **`tdarr-node`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${STORAGE_ROOT}/server:/app/server
${STORAGE_ROOT}/config:/app/configs
${STORAGE_ROOT}/log:/app/logs
${TEMP_ROOT}:/temp
${MEDIA_ROOT}/:/media
${MEDIA_ROOT}/Movies:/output/movies
${MEDIA_ROOT}/Tv:/output/tv
${STORAGE_ROOT}/config:/app/configs
${STORAGE_ROOT}/log:/app/logs
${TEMP_ROOT}:/temp
${MEDIA_ROOT}/:/media
${MEDIA_ROOT}/Movies:/output/movies
${MEDIA_ROOT}/Tv:/output/tv
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
