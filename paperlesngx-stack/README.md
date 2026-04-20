# paperlesngx-stack

Document management — Paperless-ngx

## Services

```
  • postgres
  • redis
  • tika
  • gotenberg
  • paperless
```

## Key Env Vars

- `PAPERLESS_ALLOWED_HOSTS`
- `PAPERLESS_CSRF_TRUSTED_ORIGINS`
- `PAPERLESS_DBHOST`
- `PAPERLESS_DBNAME`
- `PAPERLESS_DBPASS`
- `PAPERLESS_DBUSER`
- `PAPERLESS_ENABLE_TRASH`
- `PAPERLESS_GOTENBERG_ENDPOINT`
- `PAPERLESS_REDIS`
- `PAPERLESS_SECRET_KEY`
- `PAPERLESS_TIKA_ENABLED`
- `PAPERLESS_TIKA_ENDPOINT`
- `PAPERLESS_TOTP_ENABLED`
- `PAPERLESS_URL`
- `POSTGRES_DB`

## Volumes

- `/mnt/storagepool/apps_config/paperless_ngx/postgres/17/docker`
- `/mnt/storagepool/apps_config/paperless_ngx/data`
- `/mnt/storagepool/apps_config/paperless_ngx/media`
- `/mnt/storagepool/apps_config/paperless_ngx/consume`
- `/mnt/storagepool/apps_config/paperless_ngx/trash`

## Ports

- `30070`

## Deployment

```bash
cd paperlesngx-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration