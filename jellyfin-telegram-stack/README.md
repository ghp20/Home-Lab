# jellyfin-telegram-stack

Jellyfin Telegram bot

## Stack: jellyfin-telegram-stack

### Services

```
  • jellyfin-telegram
```

### Key Environment Variables

- `JELLYFIN_API_KEY`
- `JELLYFIN_URL`
- `TELEGRAM_CHAT_ID`
- `TELEGRAM_TOKEN`

### Volumes

- `/mnt/storagepool/scripts/jellyfin-telegram`

### Deployment

```bash
cd jellyfin-telegram-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
