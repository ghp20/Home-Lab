# beszel-stack

Server monitoring — Beszel

## Services

```
  • beszel
  • beszel-agent
```

## Volumes

- `/var/run/docker.sock`

## Deployment

```bash
cd beszel-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration