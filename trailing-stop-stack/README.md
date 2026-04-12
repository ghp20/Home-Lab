# trailing-stop-stack

Docker Compose stack for **trailing-stop-stack**.

## Services

| Service | Image |
|---------|-------|
| db | `postgres:16` |
| agent | `trailing_stop_agent:latest` |

## Environment Variables

All secrets are referenced via `${VAR}` placeholders. Create a `.env` file or set them in your Portainer stack configuration.

- `ALPACA_API_KEY` — replace with actual value
- `ALPACA_PAPER` — replace with actual value
- `DB_HOST` — see compose for default
- `DB_NAME` — replace with actual value
- `DB_POOL_MAX` — replace with actual value
- `DB_POOL_MIN` — replace with actual value
- `DB_PORT` — see compose for default
- `DB_SSLMODE` — see compose for default
- `DB_USER` — replace with actual value
- `EMA_FAST` — replace with actual value
- `EMA_SLOW` — replace with actual value
- `HOST_IP` — replace with actual value
- `INTRADAY_SCAN_COUNT` — replace with actual value
- `LOG_DIR` — replace with actual value
- `LOG_LEVEL` — replace with actual value
- `MARKET_TIMEZONE` — replace with actual value
- `MAX_DAILY_LOSS` — replace with actual value
- `MAX_DRAWDOWN` — replace with actual value
- `MAX_POSITIONS` — replace with actual value
- `MIN_AVG_VOLUME` — replace with actual value
- `MIN_STOCK_PRICE` — replace with actual value
- `N8N_MIN_SEVERITY` — replace with actual value
- `N8N_WEBHOOK_SECRET` — replace with actual value
- `N8N_WEBHOOK_URL` — replace with actual value
- `NOTIFY_RATE_LIMIT_SECS` — replace with actual value
- `PGDATA` — see compose for default
- `POSTGRES_DB` — replace with actual value
- `POSTGRES_USER` — replace with actual value
- `PRINCIPAL` — replace with actual value
- `RSI_HIGH` — replace with actual value
- `RSI_LOW` — replace with actual value
- `RSI_PERIOD` — replace with actual value
- `SPY_MA_PERIOD` — replace with actual value
- `SPY_REGIME_FILTER` — replace with actual value
- `STOP_UPDATE_INTERVAL_SECS` — replace with actual value
- `TELEGRAM_BOT_TOKEN` — replace with actual value
- `TELEGRAM_CHAT_ID` — replace with actual value
- `TRAIL_PERCENT` — replace with actual value
- `VOLUME_MA_PERIOD` — replace with actual value

## Volumes

- /path/to/your/data

## Networks

trading_net

## Notes

- Deploy via Portainer or `docker compose up -d`
- Update all `${VAR}` placeholders with actual values before deploying
- Adjust volume paths to match your storage layout
