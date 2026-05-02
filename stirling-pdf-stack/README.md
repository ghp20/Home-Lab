# stirling-pdf-stack

> Web-based PDF toolkit — merge, split, convert, OCR, sign PDFs

**Status:** 🟢 Active | **Portainer ID:** 2 | **Category:** 🖥 Infrastructure & Monitoring

---

## 📖 Overview

Web-based PDF toolkit — merge, split, convert, OCR, sign PDFs.

This stack is part of the [🖥 Infrastructure & Monitoring](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`stirling-pdf`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
/path/to/data/apps_config/stirlingpdf/tesseract_data:/usr/share/tessdata
/path/to/data/apps_config/stirlingpdf/config:/configs
/path/to/data/apps_config/stirlingpdf/files_storage:/output
/path/to/data/apps_config/stirlingpdf/logs:/logs
/path/to/data/apps_config/stirlingpdf/pipeline:/pipeline
```

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
