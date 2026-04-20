# tugtainer-stack

Docker management UI

## Stack: tugtainer-stack

### Services

```
  • app
```

### Volumes

- `/var/run/docker.sock`
- `/mnt/storagepool/apps_config/tugtainer/config`

### Deployment

```bash
cd tugtainer-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
