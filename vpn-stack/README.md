# vpn-stack

VPN download stack — Gluetun VPN, qBittorrent, SABnzbd, BitMagnet

## Stack: vpn-stack

### Services

```
  • arrnet
  • options
  • gluetun
  • qbittorrent
  • sabnzbd
  • postgres-bitmagnet
  • bitmagnet-process
  • bitmagnet-worker
```

### Key Environment Variables

- `BITMAGNET__HTTP__ADDR`
- `BITMAGNET__HTTP__ENABLED`
- `BLOCK_MALICIOUS`
- `CONTROL_SERVER_ADDRESS`
- `DNS_ADDRESS`
- `DNS_KEEP_NAMESERVER`
- `DOT`
- `FIREWALL`
- `FIREWALL_INPUT_PORTS`
- `FIREWALL_OUTBOUND_SUBNETS`
- `HEALTH_TARGET_ADDRESS`
- `PGID`
- `POSTGRES_DB`
- `POSTGRES_DSN`
- `POSTGRES_PASSWORD`

### Volumes

- `/dev/net/tun`
- `/mnt/storagepool/apps_config/gluetun`
- `/mnt/storagepool/apps_config/qbittorrent/config`
- `/mnt/storagepool/master/Media/downloads`
- `/mnt/storagepool/apps_config/sabnzbd/config`
- `/mnt/storagepool/media/usenet_incomplete`

### Ports Exposed

- `8085`
- `6881`
- `6881`
- `3333`
- `8089`

### Deployment

```bash
cd vpn-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
