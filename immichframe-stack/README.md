# immichframe-stack

Photo frame — Immich Frame

## Services

```
  • immichframe
```

## Key Env Vars

- `PLAYBACK_MODE`
- `TZ`

## Volumes

- `/mnt/storagepool/apps_config/immichframe/cache`

## Ports

- `30042`

## Deployment

```bash
cd immichframe-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration