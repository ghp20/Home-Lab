# tracktor-stack

Docker stack managed by Portainer

## Services

```
  • app
```

## Deployment

```bash
cd tracktor-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration