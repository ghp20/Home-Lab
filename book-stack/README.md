# book-stack

> Complete book stack — Calibre, Audiobookshelf, Calibre-Web for ebooks & audiobooks

**Status:** 🟢 Active | **Portainer ID:** 301 | **Category:** 📦 Productivity & Collaboration

---

## 📖 Overview

Complete book stack — Calibre, Audiobookshelf, Calibre-Web for ebooks & audiobooks.

This stack is part of the [📦 Productivity & Collaboration](#) category in my homelab. See the [root README](../README.md) for full server details and the complete stack index.

## 🧩 Services

- **`books_net`**
- **`bookshelf`**
- **`calibre`**
- **`calibre-web`**
- **`audiobookshelf`**
- **`calibre-importer`**

## 📁 Volumes & Data

This stack uses Docker volumes and bind mounts as defined in the compose file. Key mount points:

```
/path/to/data/apps_config/calibre/config:/config
/path/to/data/master/Media/Books/ebooks:/books/ebooks
/path/to/data/apps_config/calibre/inbox:/inbox
/path/to/data/apps_config/calibre-web/config:/config
/path/to/data/master/Media/Books/ebooks:/books
/path/to/data/apps_config/audiobookshelf/config:/config
/path/to/data/apps_config/audiobookshelf/metadata:/metadata
/path/to/data/master/Media/Books/audiobooks:/audiobooks
/path/to/data/master/Media/Books/ebooks:/books
/path/to/data/master/Media/Books/ebooks:/incoming
/path/to/data/scripts/calibre-importer:/scripts
/path/to/data/apps_config/calibre-importer:/config
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
