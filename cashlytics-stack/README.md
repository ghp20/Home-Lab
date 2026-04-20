# cashlytics-stack

Docker stack managed by Portainer

## Services

```
  • postgres
  • cashlytics
  • cashlytics-cron
```

## Key Env Vars

- `AUTH_SECRET`
- `AUTH_TRUST_HOST`
- `CRON_SECRET`
- `DATABASE_URL`
- `NEXT_PUBLIC_APP_URL`
- `NEXT_PUBLIC_DEFAULT_CURRENCY`
- `NEXT_PUBLIC_DEFAULT_LOCALE`
- `OPENAI_API_KEY`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `SINGLE_USER_EMAIL`
- `SINGLE_USER_MODE`

## Volumes

- `/mnt/storagepool/apps_config/cashlytics/postgres`

## Ports

- `3050`

## Deployment

```bash
cd cashlytics-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration