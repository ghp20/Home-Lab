# firefly3-stack

Personal finance — Firefly III

## Services

```
  • firefly-db
  • firefly-iii
  • firefly-importer
```

## Key Env Vars

- `APP_KEY`
- `APP_URL`
- `DB_CONNECTION`
- `DB_DATABASE`
- `DB_HOST`
- `DB_PASSWORD`
- `DB_PORT`
- `DB_USERNAME`
- `FIREFLY_III_ACCESS_TOKEN`
- `FIREFLY_III_URL`
- `MYSQL_DATABASE`
- `MYSQL_PASSWORD`
- `MYSQL_ROOT_PASSWORD`
- `MYSQL_USER`
- `TRUSTED_PROXIES`

## Deployment

```bash
cd firefly3-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration