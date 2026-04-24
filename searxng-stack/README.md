# searxng-stack

Privacy-respecting metasearch — SearXNG

## Services

```
  • redis
  • searxng
```

## Deployment

```bash
cd searxng-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration