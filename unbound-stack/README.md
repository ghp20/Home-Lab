# unbound-stack

DNS resolver — Unbound

## Services

```
  • unbound
```

## Deployment

```bash
cd unbound-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration