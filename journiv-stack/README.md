# journiv-stack

Personal journal/writing platform

## Services

```
  • options
  • postgres
  • redis
  • celery-worker
  • app
  • backend
  • frontend
```

## Key Env Vars

- `CELERY_BROKER_URL`
- `CELERY_RESULT_BACKEND`
- `DB_DRIVER`
- `DOMAIN_NAME`
- `ENVIRONMENT`
- `POSTGRES_DB`
- `POSTGRES_HOST`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `RATE_LIMIT_STORAGE_URI`
- `REDIS_URL`
- `SECRET_KEY`
- `SERVICE_ROLE`

## Volumes

- `/var/run/postgresql`
- `/mnt/storagepool/apps_config/journiv/postgres_data`
- `/mnt/storagepool/apps_config/journiv/redis_data`
- `/mnt/storagepool/apps_config/journiv/app_data`
- `/mnt/storagepool/apps_config/journiv/app_data`

## Ports

- `8000`

## Deployment

```bash
cd journiv-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration