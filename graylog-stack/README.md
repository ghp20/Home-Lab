# graylog-stack

Log management — Graylog

## Stack: graylog-stack

### Services

```
  • graylog_net
  • mongodb
  • datanode
  • graylog
```

### Key Environment Variables

- `GRAYLOG_DATANODE_HTTP_EXTERNAL_URI`
- `GRAYLOG_DATANODE_MONGODB_URI`
- `GRAYLOG_DATANODE_NODE_ID_FILE`
- `GRAYLOG_DATANODE_OPENSEARCH_HEAP`
- `GRAYLOG_DATANODE_PASSWORD_SECRET`
- `GRAYLOG_HTTP_EXTERNAL_URI`
- `GRAYLOG_MONGODB_URI`
- `GRAYLOG_PASSWORD_SECRET`

### Volumes

- `/mnt/storagepool/apps_config/graylog/mongodb-data`
- `/mnt/storagepool/apps_config/graylog/datanode-data`
- `/mnt/storagepool/apps_config/graylog/graylog-data`

### Ports Exposed

- `8999`
- `9000`
- `12201`
- `12201`
- `5140`
- `5140`

### Deployment

```bash
cd graylog-stack
docker compose up -d
```

### Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as environment variables via Portainer stack
- See `docker-compose.yaml` for full configuration
