# 🐳 Docker Compose Cheat Sheet

## 🔧 Basic Commands
```bash
docker-compose up            # Start all services
docker-compose up -d         # Start in detached mode
docker-compose down          # Stop and remove services
docker-compose ps            # List services
docker-compose logs          # Show logs
```

## ⚙️ Example docker-compose.yml
```yaml
version: "3.8"
services:
  web:
    build: .
    ports:
      - "3000:3000"
    volumes:
      - .:/app
  db:
    image: postgres
    environment:
      POSTGRES_PASSWORD: example
```

## 🧪 Tips
- Use `.env` files for config
- `docker-compose -f custom.yml up` for alt configs