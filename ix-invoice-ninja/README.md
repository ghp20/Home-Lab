# Ix-Invoice-Ninja — TrueNAS SCALE Managed

> ⚠️ **TrueNAS SCALE managed app.** Do NOT deploy via Portainer.
**Generated:** 2026-04-19 21:26

| Service | Image |
|---------|-------|
| `ix-invoice-ninja-scheduler-1` | `invoiceninja/invoiceninja-octane:5.12.28-o` |
| `ix-invoice-ninja-worker-1` | `invoiceninja/invoiceninja-octane:5.12.28-o` |
| `ix-invoice-ninja-invoice-ninja-1` | `invoiceninja/invoiceninja-octane:5.12.28-o` |
| `ix-invoice-ninja-mariadb-1` | `mariadb:12.2.2` |
| `ix-invoice-ninja-redis-1` | `valkey/valkey:9.0.3` |

## Notes
- All secrets sanitized to `${{VAR}}` placeholders
