# portracker-stack

Port tracking dashboard

## Stack: portracker-stack

### Services

```
  • portracker
```

### Key Environment Variables

- `DATABASE_PATH`
- `PORT`
- `TRUENAS_API_KEY`
- `TRUENAS_WS_BASE`

### Volumes

- `/mnt/storagepool/apps_config/portracker/data`
- `/var/run/docker.sock`

### Deployment

```bash
cd portracker-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
