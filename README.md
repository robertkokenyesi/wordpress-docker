# WordPress + MySQL Docker Compose Setup

Simple, clean Docker Compose stack for **WordPress** + **MySQL** — suitable for local development, testing or small sites.

Runs WordPress on port 85[](http://localhost:85) so it doesn't conflict with other local web servers.

## Features

- Official `wordpress:latest` and `mysql:latest` images
- Persistent data via local folders
- All credentials managed via `.env` file (never committed)
- UTF-8 ready database
- Easy to extend for plugin/theme development (commented lines ready)

## Quick Start (local usage)

1. Clone the repo
   ```bash
   git clone https://github.com/robertkokenyesi/wordpress-docker.git
   cd wordpress-docker
2. Prepare environment file
    cp .env.example .env
    nano .env #change all values to secure ones!
3. Start container
    docker compose -f docker-compose.yml up -d
4. Open in browser:
    WordPress: http://localhost:85
    First install wizard should appear
5. Stop docker compose down # if need
