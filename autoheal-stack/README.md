# autoheal-stack

Docker stack managed by Portainer

## Services

```
  • autoheal
```

## Deployment

```bash
cd autoheal-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration