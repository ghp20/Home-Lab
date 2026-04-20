# adventurlog-stack

Adventure logging

## Stack: adventurlog-stack

### Services

```
  • options
  • db
  • backend
  • frontend
```

### Key Environment Variables

- `BODY_SIZE_LIMIT`
- `CSRF_TRUSTED_ORIGINS`
- `DEBUG`
- `DJANGO_ADMIN_EMAIL`
- `DJANGO_ADMIN_PASSWORD`
- `DJANGO_ADMIN_USERNAME`
- `FRONTEND_PORT`
- `FRONTEND_URL`
- `ORIGIN`
- `PGHOST`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `PUBLIC_SERVER_URL`
- `PUBLIC_URL`

### Volumes

- `/mnt/storagepool/apps_config/adventurelog/.env`
- `/mnt/storagepool/apps_config/postgres`
- `/mnt/storagepool/apps_config/adventurelog/.env`
- `/mnt/storagepool/apps_config/media`

### Ports Exposed

- `8016`
- `8015`

### Deployment

```bash
cd adventurlog-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
