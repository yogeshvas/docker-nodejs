Here’s your enhanced Docker notes formatted as a **GitHub README.md** file:

````markdown
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
````

---

## 🧰 Inside the Ubuntu Container

```bash
apt update         # Update package lists
apt install vim    # Install Vim editor
```

---

## 🐳 Working with Alpine (Lightweight Image)

```bash
# Pull and run Alpine image
docker pull alpine
docker run -it alpine

# Inside the container
apk update         # Update Alpine packages
apk add vim        # Install Vim
```

---

## 🌐 Port Mapping

```bash
# Map port 7990 on host to port 80 in the container
docker run -it -p 7990:80 nginx
```

> 📌 **Syntax:** `-p <hostPort>:<containerPort>`

---

## 📄 Viewing Logs & Accessing Containers

```bash
docker logs <CONTAINER_ID>             # View container logs
docker exec -it <CONTAINER_ID> bash    # Start a shell session inside the container
```

---

## 🛠️ Creating a Custom Docker Image

1. Create a file named `Dockerfile` with the following contents:

```Dockerfile
FROM python
ADD app.py /tree/app.py
CMD ["python", "/tree/app.py"]
```

2. Build the Docker image:

```bash
docker build -t python-hello-world .
```

---

## 🧹 Cleaning Up

```bash
# Remove all dangling (unused) images
docker image prune
```

---

## 📁 File Structure Example

```
your-project/
│
├── Dockerfile
└── app.py
```

---

## 📚 Resources

* [Official Docker Documentation](https://docs.docker.com/)
* [Docker Hub](https://hub.docker.com/)

```

You can save this content as your `README.md` in your GitHub repository. Let me know if you want to include visuals or a Docker diagram!
```
