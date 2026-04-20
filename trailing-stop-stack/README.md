# trailing-stop-stack

Trading bot — Alpaca API, PostgreSQL

## Services

```
  • trading_net
  • db
  • agent
```

## Volumes

- `/mnt/storagepool/apps_config/ron/trailing-stop/postgres/pgdata`
- `/mnt/storagepool/apps_config/ron/trailing-stop/logs`
- `/mnt/storagepool/apps_config/ron/trailing-stop/backtest`

## Ports

- `5433`

## Deployment

```bash
cd trailing-stop-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration