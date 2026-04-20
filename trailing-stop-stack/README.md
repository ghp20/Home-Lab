# trailing-stop-stack

Trailing stop trading bot

## Stack: trailing-stop-stack

### Services

```
  • trading_net
  • db
  • agent
```

### Key Environment Variables

- `ALPACA_API_KEY`
- `ALPACA_PAPER`
- `ALPACA_SECRET_KEY`
- `DB_HOST`
- `DB_NAME`
- `DB_PASSWORD`
- `DB_POOL_MAX`
- `DB_POOL_MIN`
- `DB_PORT`
- `DB_SSLMODE`
- `DB_USER`
- `EMA_FAST`
- `EMA_SLOW`
- `EQUITY_CAP`
- `HOST_IP`

### Volumes

- `/mnt/storagepool/apps_config/ron/trailing-stop/postgres/pgdata`
- `/mnt/storagepool/apps_config/ron/trailing-stop/logs`
- `/mnt/storagepool/apps_config/ron/trailing-stop/backtest`

### Ports Exposed

- `5433`

### Deployment

```bash
cd trailing-stop-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
