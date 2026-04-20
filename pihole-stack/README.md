# pihole-stack

Network-wide ad blocking — Pi-hole

## Stack: pihole-stack

### Services

```
  • pihole
```

### Key Environment Variables

- `TZ`
- `WEB_PORT`

### Volumes

- `/mnt/storagepool/apps_config/pihole/etc-pihole`
- `/mnt/storagepool/apps_config/pihole/etc-dnsmasq.d`

### Deployment

```bash
cd pihole-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
