# wygiwyh-stack

AI image generation UI

## Services

```
  • db
  • wygiwyh
```

## Key Env Vars

- `ADMIN_EMAIL`
- `ADMIN_PASSWORD`
- `DEBUG`
- `DJANGO_ALLOWED_HOSTS`
- `ENABLE_SOFT_DELETE`
- `HTTPS_ENABLED`
- `KEEP_DELETED_TRANSACTIONS_FOR`
- `OUTBOUND_PORT`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `SECRET_KEY`
- `SQL_DATABASE`
- `SQL_HOST`
- `SQL_PASSWORD`

## Volumes

- `/mnt/storagepool/apps_config/wygiwyh/db`
- `/mnt/storagepool/apps_config/wygiwyh/media`
- `/mnt/storagepool/apps_config/wygiwyh/static`

## Ports

- `9711`

## Deployment

```bash
cd wygiwyh-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration