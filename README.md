## 👋 Welcome to tududi 🚀

Minimalist to-do and task management application

## 📋 Description

Minimalist to-do and task management application

## 🚀 Services

- **app**: chrisvel/tududi:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/tududi/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/tududi" ~/.local/srv/docker/tududi
cd ~/.local/srv/docker/tududi
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install tududi
```

## 🔧 Configuration

### Environment Variables

```shell
APP_USER_PASS=password
APP_USER_NAME=admin
APP_SECRET_TOKEN_32=0B1Xo65hlCWCDeV9XjSilSSn4JbbXAyo
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:59088

## 📂 Volumes

- `./rootfs/data/tududi` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
