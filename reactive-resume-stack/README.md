# reactive-resume-stack

Resume builder — Reactive Resume

## Stack: reactive-resume-stack

### Services

```
  • postgres
  • printer
  • app
```

### Key Environment Variables

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

### Volumes

- `/mnt/storagepool/apps_config/reactive-resume/db`
- `/mnt/storagepool/apps_config/reactive-resume/data`

### Ports Exposed

- `30120`

### Deployment

```bash
cd reactive-resume-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
