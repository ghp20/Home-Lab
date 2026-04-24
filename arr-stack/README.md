# arr-stack

Media management — Prowlarr, Radarr, Sonarr, Bazarr, Lazylibrarian, CleanupArr

## Services

```
  • options
  • arrnet
  • prowlarr
  • radarr
  • sonarr
  • bazarr
  • lazylibrarian
  • cleanuparr
```

## Key Env Vars

- `PGID`
- `PUID`
- `TZ`

## Deployment

```bash
cd arr-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration