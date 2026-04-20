# tandoor-recipes-stack

Recipe manager — Tandoor

## Stack: tandoor-recipes-stack

### Services

```
  • postgres
  • tandoor
```

### Key Environment Variables

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

### Volumes

- `/mnt/storagepool/apps_config/tandoor-recipes/postgres`
- `/mnt/storagepool/apps_config/tandoor-recipes/files`
- `/mnt/storagepool/apps_config/tandoor-recipes/media`

### Ports Exposed

- `9925`

### Deployment

```bash
cd tandoor-recipes-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
