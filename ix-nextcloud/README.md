# Ix-Nextcloud — TrueNAS SCALE Managed

> ⚠️ **TrueNAS SCALE managed app.** Do NOT deploy via Portainer.
**Generated:** 2026-04-19 21:26

| Service | Image |
|---------|-------|
| `ix-nextcloud-cron-1` | `ix-nextcloud:33.0.2_2d91b2869075cb02556af5819ab2fc278f4bcf751f535ea675c8104091781dba` |
| `ix-nextcloud-nginx-1` | `nginx:1.29.8` |
| `ix-nextcloud-nextcloud-1` | `ix-nextcloud:33.0.2_2d91b2869075cb02556af5819ab2fc278f4bcf751f535ea675c8104091781dba` |
| `ix-nextcloud-postgres-1` | `postgres:17.9-bookworm` |
| `ix-nextcloud-redis-1` | `valkey/valkey:9.0.3` |
| `ix-nextcloud-imaginary-1` | `ghcr.io/nextcloud-releases/aio-imaginary:20260409_094910` |

## Notes
- All secrets sanitized to `${{VAR}}` placeholders
