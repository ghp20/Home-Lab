# vaultwarden-stack

Password manager — VaultWarden

## Services

```
  • db
  • vaultwarden
  • vaultwarden-net
```

## Key Env Vars

- `ADMIN_TOKEN`
- `DATABASE_URL`
- `DOMAIN`
- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`
- `ROCKET_PORT`
- `WEBSOCKET_ENABLED`

## Deployment

```bash
cd vaultwarden-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration