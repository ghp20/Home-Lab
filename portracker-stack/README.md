# portracker-stack

Port tracking dashboard

## Services

```
  • portracker
```

## Deployment

```bash
cd portracker-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration