# tandoor-recipes-stack

Recipe manager — Tandoor

## Services

```
  • postgres
  • tandoor
```

## Key Env Vars

- `AI_ENABLE`
- `AI_PROVIDER`
- `ALLOWED_HOSTS`
- `COMMENT_PREF_DEFAULT`
- `DB_ENGINE`
- `DEBUG`
- `FRACTION_PREF_DEFAULT`
- `GUNICORN_MEDIA`
- `OPENAI_API_KEY`
- `OPENAI_MODEL`
- `PGDATA`
- `POSTGRES_DB`
- `POSTGRES_HOST`
- `POSTGRES_PASSWORD`
- `POSTGRES_PORT`

## Deployment

```bash
cd tandoor-recipes-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration