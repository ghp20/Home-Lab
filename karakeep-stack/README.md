# karakeep-stack

Docker stack managed by Portainer

## Services

```
  • options
  • web
  • chrome
  • meilisearch
```

## Key Env Vars

- `BROWSER_WEB_URL`
- `DATA_DIR`
- `MEILI_ADDR`
- `MEILI_NO_ANALYTICS`
- `NEXTAUTH_SECRET`
- `NEXTAUTH_URL`
- `OPENAI_API_KEY`

## Deployment

```bash
cd karakeep-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration