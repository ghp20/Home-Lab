# adventurlog-stack

Docker stack managed by Portainer

## Services

```
  • options
  • db
  • backend
  • frontend
```

## Key Env Vars

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

## Deployment

```bash
cd adventurlog-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration