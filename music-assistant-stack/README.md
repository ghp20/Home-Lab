# music-assistant-stack

Docker stack managed by Portainer

## Services

```
  • music-assistant-server
```

## Ports

- `8095`

## Deployment

```bash
cd music-assistant-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration