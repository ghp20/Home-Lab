# karakeep-stack

Bookmark keeper — Karakeep

## Stack: karakeep-stack

### Services

```
  • options
  • web
  • chrome
  • meilisearch
```

### Key Environment Variables

- `BROWSER_WEB_URL`
- `DATA_DIR`
- `MEILI_ADDR`
- `MEILI_NO_ANALYTICS`
- `NEXTAUTH_SECRET`
- `NEXTAUTH_URL`
- `OPENAI_API_KEY`

### Volumes

- `/mnt/storagepool/apps_config/karakeep/data`
- `/mnt/storagepool/apps_config/karakeep/meilisearch`

### Ports Exposed

- `30147`

### Deployment

```bash
cd karakeep-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
