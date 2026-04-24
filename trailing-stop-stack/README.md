# trailing-stop-stack

Trading bot — Alpaca API, PostgreSQL

## Services

```
  • trading_net
  • db
  • agent
```

## Deployment

```bash
cd trailing-stop-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration