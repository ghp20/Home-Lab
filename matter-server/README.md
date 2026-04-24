# matter-server

Docker stack managed by Portainer

## Services

```
  • matter-server
```

## Deployment

```bash
cd matter-server
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration