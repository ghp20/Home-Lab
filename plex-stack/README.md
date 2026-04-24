# plex-stack

Media server — Plex

## Services

```
  • plex
```

## Volumes

- `/dev/dri`

## Deployment

```bash
cd plex-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration