# jellyfin-telegram-stack

Docker stack managed by Portainer

## Services

```
  • jellyfin-telegram
```

## Key Env Vars

- `JELLYFIN_API_KEY`
- `JELLYFIN_URL`
- `TELEGRAM_CHAT_ID`
- `TELEGRAM_TOKEN`

## Deployment

```bash
cd jellyfin-telegram-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration