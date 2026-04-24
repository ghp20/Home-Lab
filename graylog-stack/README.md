# graylog-stack

Log management — Graylog

## Services

```
  • graylog_net
  • mongodb
  • datanode
  • graylog
```

## Key Env Vars

- `GRAYLOG_DATANODE_HTTP_EXTERNAL_URI`
- `GRAYLOG_DATANODE_MONGODB_URI`
- `GRAYLOG_DATANODE_NODE_ID_FILE`
- `GRAYLOG_DATANODE_OPENSEARCH_HEAP`
- `GRAYLOG_DATANODE_PASSWORD_SECRET`
- `GRAYLOG_HTTP_EXTERNAL_URI`
- `GRAYLOG_MONGODB_URI`
- `GRAYLOG_PASSWORD_SECRET`

## Deployment

```bash
cd graylog-stack
docker compose up -d
```

## Notes

- Managed by **Portainer** on TrueNAS SCALE
- All secrets injected as env vars via Portainer stack
- See `docker-compose.yaml` for full configuration