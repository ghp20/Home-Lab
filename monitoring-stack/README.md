# monitoring-stack

> Prometheus + Grafana — full system and container monitoring

**Status:** 🟢 Active | **Portainer ID:** 156 | **Category:** 🖥 Infrastructure & Monitoring

---

## 📖 Overview

Prometheus + Grafana — full system and container monitoring.

This stack is part of the [🖥 Infrastructure & Monitoring](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`prometheus`**
- **`grafana`**
- **`monitoring-net`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
${STORAGE_ROOT}/prometheus/config/prometheus.yml:/etc/prometheus/prometheus.yml:ro
${STORAGE_ROOT}/prometheus/data:/prometheus
${STORAGE_ROOT}/grafana/data:/var/lib/grafana
```

## ⚠️ Gotchas & Tips

⚠️ Prometheus TSDB grows continuously — set retention policies (default 15d)

⚠️ High-cardinality metric labels can crash Prometheus under memory pressure

⚠️ Grafana admin password is set on first login — change it immediately

⚠️ No built-in alerting — AlertManager must be added separately for notifications


## 🚀 Deployment

1. **Review** the `docker-compose.yaml` file and update all `changeme` placeholder values
2. **Adjust** volume paths to match your storage layout
3. **Configure** environment variables — see the compose file for all options
4. **Deploy** using Portainer or Docker Compose:

```bash
docker compose -f docker-compose.yaml up -d
```

5. **Verify** containers are running:

```bash
docker compose -f docker-compose.yaml ps
```

## 🔗 Related Stacks

See the [root README](../README.md) for the full stack index organized by category.

---

*📝 README maintained as part of the Home-Lab repository. Last updated: {datetime.now().strftime('%Y-%m-%d')}*
