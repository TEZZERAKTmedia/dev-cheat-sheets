
# 🐳 Docker Command Cheat Sheet (Ordered by Usage)

This cheat sheet is organized from **most common** to **least common** Docker commands to help you efficiently manage containers, images, and environments.

---

## ✅ Most Common Docker Commands (Daily Use)

### 🛠️ Basic Workflow
```bash
docker build -t name .         # Build image from Dockerfile
docker run name                # Run container from image
docker ps                      # List running containers
docker stop <container_id>     # Stop a running container
docker start <container_id>    # Start a stopped container
```

### 🗂️ Image and Container Management
```bash
docker images                  # List local images
docker rmi <image_id>          # Remove image
docker rm <container_id>       # Remove stopped container
```

---

## 🔧 Intermediate Commands (Weekly Use)

### 🔁 Working with Containers
```bash
docker exec -it <container_id> bash # Access shell inside container
docker logs <container_id>          # View logs from container
docker cp <container_id>:src dst    # Copy file from container to host
```

### 📦 Volumes and Ports
```bash
docker run -v host:container name      # Mount volume
docker run -p host:container name      # Map ports
```

---

## 🧪 Less Common (Advanced or Fixes)

### 🐳 Docker Compose
```bash
docker-compose up -d       # Start services in the background
docker-compose down        # Stop and remove services
docker-compose logs        # Show logs
```

### 🔍 Inspecting and Debugging
```bash
docker inspect <id>        # Detailed container/image info
docker diff <container_id> # Check filesystem changes
docker history <image_id>  # Show image build history
```

---

## 🧙‍♂️ Rare or Specialized Commands

### 🧼 Cleanup
```bash
docker system prune        # Remove unused data
docker volume prune        # Remove unused volumes
docker network prune       # Remove unused networks
```

### 🧰 Misc
```bash
docker tag src dst         # Tag image
docker save -o file.tar img # Save image to tarball
docker load -i file.tar    # Load image from tarball
```

---

Happy Dockering! 🐋
