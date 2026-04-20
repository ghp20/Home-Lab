# Ix-Immich — TrueNAS SCALE Managed

> ⚠️ **TrueNAS SCALE managed app.** Do NOT deploy via Portainer.
> Auto-generated from `docker inspect` on the homelab.

**Generated:** 2026-04-19 21:11

| Service | Image |
|---------|-------|
| `learning_1` | `ghcr.io/immich-app/immich-machine-learning:v2.7.3-cuda` |
| `immich_pgvecto_1` | `ghcr.io/immich-app/postgres:18-vectorchord0.5.3` |
| `immich_redis_1` | `valkey/valkey:9.0.3` |
| `immich_server_1` | `ghcr.io/immich-app/immich-server:v2.7.3` |

## Notes
- All secrets sanitized to `${{VAR}}` placeholders
- Managed by TrueNAS SCALE App Catalog
