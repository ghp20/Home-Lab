# mealie-stack

Recipe manager — Mealie

## Stack: mealie-stack

### Services

```
  • postgres
  • mealie
  • default
```

### Key Environment Variables

- `ALLOW_SIGNUP`
- `BASE_URL`
- `DB_ENGINE`
- `OPENAI_API_KEY`
- `OPENAI_MAX_TOKENS`
- `OPENAI_MODEL`
- `OPENAI_TEMPERATURE`
- `PGID`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_PORT`
- `POSTGRES_SERVER`
- `POSTGRES_USER`
- `PUID`
- `SMTP_FROM_EMAIL`

### Volumes

- `/mnt/storagepool/apps_config/mealie/postgres`
- `/mnt/storagepool/apps_config/mealie/mealie/data`

### Ports Exposed

- `9926`

### Deployment

```bash
cd mealie-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
