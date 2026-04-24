# lubelogger-stack

Docker stack managed by Portainer

## Services

```
  • lubelogger
```

## Key Env Vars

- `ASPNETCORE_DATAPROTECTION__DIRECTORY`
- `ASPNETCORE_URLS`
- `PGID`
- `PUID`
- `TZ`

## Deployment

```bash
cd lubelogger-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration