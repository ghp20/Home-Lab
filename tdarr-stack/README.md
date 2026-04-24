# tdarr-stack

Media transcoding — Tdarr

## Services

```
  • tdarr
  • tdarr-node
```

## Volumes

- `/dev/dri/renderD128`
- `/dev/dri/card0`
- `/dev/dri/renderD128`
- `/dev/dri/card0`

## Deployment

```bash
cd tdarr-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration