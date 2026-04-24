# vpn-stack

VPN download stack — Gluetun, qBittorrent, SABnzbd, BitMagnet

## Services

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

## Key Env Vars

- `POSTGRES_DB`
- `POSTGRES_PASSWORD`
- `POSTGRES_USER`

## Ports

- `8085`
- `6881`
- `6881`
- `3333`
- `8089`

## Deployment

```bash
cd vpn-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration