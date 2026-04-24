# npm-stack

Reverse proxy — Nginx Proxy Manager

## Services

```
  • npm
```

## Deployment

```bash
cd npm-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration