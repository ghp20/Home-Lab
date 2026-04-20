# reactive-resume-stack

Docker stack managed by Portainer

## Services

```
  • postgres
  • printer
  • app
```

## Key Env Vars

- `APP_URL`
- `AUTH_SECRET`
- `CONCURRENT`
- `DATABASE_URL`
- `FLAG_DEBUG_PRINTER`
- `FLAG_DISABLE_EMAIL_AUTH`
- `FLAG_DISABLE_SIGNUPS`
- `HEALTH`
- `NODE_ENV`
- `PORT`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `PRINTER_ENDPOINT`
- `SMTP_FROM`

## Volumes

- `/mnt/storagepool/apps_config/reactive-resume/db`
- `/mnt/storagepool/apps_config/reactive-resume/data`

## Ports

- `30120`

## Deployment

```bash
cd reactive-resume-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration