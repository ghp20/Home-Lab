# timelinize-stack

Docker stack managed by Portainer

## Services

```
  • timelinize
```

## Key Env Vars

- `TLZ_ORIGIN`
- `TZ`
- `XDG_CONFIG_HOME`

## Deployment

```bash
cd timelinize-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration