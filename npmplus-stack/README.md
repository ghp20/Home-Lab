# npmplus-stack

Docker stack managed by Portainer

## Services

```
  • npmplus
  • default
  • crowdsec_net
```

## Volumes

- `/mnt/storagepool/apps_config/npmplus/data`

## Ports

- `443`
- `443`
- `8181`

## Deployment

```bash
cd npmplus-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration