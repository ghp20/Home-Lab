# seerr-stack

Media requests — Seerr

## Services

```
  • seerr-db
  • seerr
```

## Key Env Vars

- `DB_HOST`
- `DB_NAME`
- `DB_PASS`
- `DB_PORT`
- `DB_TYPE`
- `DB_USER`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `TZ`

## Volumes

- `/mnt/storagepool/apps_config/seerr/db`
- `/mnt/storagepool/apps_config/seerr/config`

## Ports

- `5055`

## Deployment

```bash
cd seerr-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration