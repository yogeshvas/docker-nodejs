# 🐳 Docker Cheat Sheet

A quick reference guide to essential Docker commands, port mapping, container management, and building custom Docker images.

---

## 📦 Basic Docker Commands

```bash
# Pull a Docker image
docker pull ubuntu

# Run a container from the image
docker run ubuntu

# Run a container with interactive terminal
docker run -it ubuntu

# List all running containers
docker ps

# List all containers (running and stopped)
docker ps -a

Inside the Ubuntu Container
apt update         # Update package lists
apt install vim    # Install Vim editor
