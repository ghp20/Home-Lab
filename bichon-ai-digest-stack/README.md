# bichon-ai-digest-stack

AI news digest

## Stack: bichon-ai-digest-stack

### Services

```
  • bichon-ai-digest
```

### Key Environment Variables

- `BICHON_ACCOUNT_IDS`
- `BICHON_TOKEN`
- `BICHON_URL`
- `MAX_EMAILS_PER_ACCOUNT`
- `MAX_ITEMS_PER_CATEGORY`
- `MAX_PAGES_PER_ACCOUNT`
- `MAX_SNIPPET_CHARS`
- `OPENAI_API_KEY`
- `OPENAI_MODEL`
- `TELEGRAM_BOT_TOKEN`
- `TELEGRAM_CHAT_ID`

### Volumes

- `/mnt/storagepool/apps_config/bichon/ai-digest`

### Deployment

```bash
cd bichon-ai-digest-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
