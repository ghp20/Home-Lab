# pihole-stack

Ad blocking — Pi-hole

## Services

```
  • pihole
```

## Key Env Vars

- `TZ`
- `WEB_PORT`

## Deployment

```bash
cd pihole-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration