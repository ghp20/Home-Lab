# mealie-stack

Recipe manager — Mealie

## Services

```
  • postgres
  • mealie
  • default
```

## Key Env Vars

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

## Deployment

```bash
cd mealie-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration