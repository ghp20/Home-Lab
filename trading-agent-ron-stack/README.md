# trading-agent-ron-stack

Trading agent (Ron profile)

## Services

```
  • trading-agent-ron
  • trading-postgres-ron
  • trading-redis-ron
  • trading-net-ron
```

## Key Env Vars

- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`

## Volumes

- `/mnt/storagepool/apps_config/ron/trading-agent-ron/config/config.yaml`
- `/mnt/storagepool/apps_config/ron/trading-agent-ron/config/.env`
- `/mnt/storagepool/apps_config/ron/trading-agent-ron/models`
- `/mnt/storagepool/apps_config/ron/trading-agent-ron/logs`
- `/mnt/storagepool/apps_config/ron/trading-agent-ron/data`
- `/mnt/storagepool/apps_config/ron/trading-agent-ron/src/`

## Ports

- `8002`
- `5434`

## Deployment

```bash
cd trading-agent-ron-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration