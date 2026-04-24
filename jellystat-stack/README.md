# jellystat-stack

Docker stack managed by Portainer

## Services

```
  • jellystat-db
  • jellystat
```

## Key Env Vars

- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `TZ`

## Deployment

```bash
cd jellystat-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration