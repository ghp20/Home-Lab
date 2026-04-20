# Ix-Nextcloud — TrueNAS SCALE Managed

> ⚠️ **TrueNAS SCALE managed app.** Do NOT deploy via Portainer.
> Auto-generated from `docker inspect` on the homelab.

**Generated:** 2026-04-19 21:11

| Service | Image |
|---------|-------|
| `nextcloud_cron_1` | `ix-nextcloud:33.0.2_2d91b2869075cb02556af5819ab2fc278f4bcf751f535ea675c8104091781dba` |
| `nextcloud_imaginary_1` | `ghcr.io/nextcloud-releases/aio-imaginary:20260409_094910` |
| `nextcloud_nextcloud_1` | `ix-nextcloud:33.0.2_2d91b2869075cb02556af5819ab2fc278f4bcf751f535ea675c8104091781dba` |
| `nextcloud_nginx_1` | `nginx:1.29.8` |
| `nextcloud_postgres_1` | `postgres:17.9-bookworm` |
| `nextcloud_redis_1` | `valkey/valkey:9.0.3` |

## Notes
- All secrets sanitized to `${{VAR}}` placeholders
- Managed by TrueNAS SCALE App Catalog
