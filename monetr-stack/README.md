# monetr-stack

Docker stack managed by Portainer

## Services

```
  • monetr
  • monetr-postgres
  • monetr-valkey
  • monetr-net
```

## Key Env Vars

- `MONETR_ALLOW_SIGN_UP`
- `MONETR_ENVIRONMENT`
- `MONETR_PG_ADDRESS`
- `MONETR_PG_DATABASE`
- `MONETR_PG_PASSWORD`
- `MONETR_PG_PORT`
- `MONETR_PG_USERNAME`
- `MONETR_REDIS_ADDRESS`
- `MONETR_REDIS_ENABLED`
- `MONETR_REDIS_PORT`
- `MONETR_SERVER_EXTERNAL_URL`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`

## Volumes

- `/mnt/storagepool/apps_config/monetr/config`
- `/mnt/storagepool/apps_config/monetr/postgres`
- `/mnt/storagepool/apps_config/monetr/valkey`

## Ports

- `4000`

## Deployment

```bash
cd monetr-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration