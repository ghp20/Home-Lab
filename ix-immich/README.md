# Ix-Immich — TrueNAS SCALE Managed

> ⚠️ **TrueNAS SCALE managed app.** Do NOT deploy via Portainer.
**Generated:** 2026-04-19 21:22

| Service | Image |
|---------|-------|
| `ix-immich-server-1` | `ghcr.io/immich-app/immich-server:v2.7.3` |
| `ix-immich-pgvecto-1` | `ghcr.io/immich-app/postgres:18-vectorchord0.5.3` |
| `ix-immich-machine-learning-1` | `ghcr.io/immich-app/immich-machine-learning:v2.7.3-cuda` |
| `ix-immich-redis-1` | `valkey/valkey:9.0.3` |

## Notes
- All secrets sanitized to `${{VAR}}` placeholders
