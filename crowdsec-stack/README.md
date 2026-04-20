# crowdsec-stack

Security — CrowdSec

## Stack: crowdsec-stack

### Services

```
  • crowdsec
  • crowdsec-cloudflare-bouncer
  • crowdsec-net
```

### Key Environment Variables

- `COLLECTIONS`
- `TZ`

### Volumes

- `/mnt/storagepool/apps_config/crowdsec/config/acquis.yaml`
- `/mnt/storagepool/apps_config/crowdsec/data`
- `/var/log`
- `/mnt/storagepool/apps_config/npm/data/logs`
- `/mnt/storagepool/apps_config/crowdsec/cloudflare-bouncer/cfg.yaml`

### Ports Exposed

- `6060`
- `1514`

### Deployment

```bash
cd crowdsec-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
