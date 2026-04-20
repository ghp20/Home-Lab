# wireguard-us-server-stack

WireGuard VPN server (US)

## Stack: wireguard-us-server-stack

### Services

```
  • options
  • wireguard-us-server
```

### Key Environment Variables

- `PGID`
- `PUID`
- `SERVERMODE`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/wireguard/server_config`
- `/lib/modules`

### Ports Exposed

- `22`
- `443`

### Deployment

```bash
cd wireguard-us-server-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
