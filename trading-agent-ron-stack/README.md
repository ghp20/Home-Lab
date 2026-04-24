# trading-agent-ron-stack

Trading agent (Ron profile)

## Services

```
  • trading-agent-ron
  • trading-postgres-ron
  • trading-redis-ron
```

## Key Env Vars

- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`

## Deployment

```bash
cd trading-agent-ron-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration