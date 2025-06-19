# 🚀 Day 15 – Docker Fundamentals | #90DaysOfDevOps

Today I explored the core fundamentals of **Docker** – a powerful containerization platform that ensures your app runs the same in every environment.

---

## 📚 Topics Covered

### 🔹 1. Why Docker?

- Traditional apps face issues when running across different machines due to environment mismatch.
- Docker solves this by packaging the app with its dependencies into a container.
- This ensures **portability**, **consistency**, and **easy deployment**.

---

### 🔹 2. Virtualization vs Containerization

| Virtualization                         | Containerization                         |
|----------------------------------------|-------------------------------------------|
| Requires full OS for every VM          | Shares host OS kernel                     |
| Heavy, slow startup                    | Lightweight and fast                      |
| Uses more RAM and disk space           | Uses only the needed resources            |
| Hypervisor manages VMs                 | Docker Engine manages containers          |

---

### 🔹 3. Installing Docker on AWS EC2

```bash
sudo apt-get install docker.io
systemctl status docker    # Check if Docker is running

```
### 🔹 4. Docker Components
- Docker Engine – the core service that creates and runs containers.

- Docker Daemon – background service that listens to Docker API requests.

- Docker CLI – tool to interact with Docker from terminal.

- Docker Images & Containers – image is a blueprint, container is the running instance.

### 🔹 5. Add User to Docker Group (No need to use sudo every time)

```bash

sudo usermod -aG docker $USER

```
### 🔹 6. Dockerfile → Image → Container

```bash
FROM openjdk:17-jdk-alpine         # Base Image
WORKDIR /app                       # Set working directory
COPY src/Main.java Main.java       # Copy Java source code
COPY quotes.txt quotes.txt         # Copy quotes file
RUN javac Main.java                # Compile Java program
EXPOSE 8000                        # Expose port
CMD ["java", "Main"]              # Run the app

```
### 🧪 Projects Deployed Using Docker
✅ Nginx Web Server container on port 80

✅ Java-based Quotes App on port 8000

✅ Python mini server on port 5000

[Previous Day →](../Day-14/README.md)                                                                                    [Next Day →](../Day-16/README.md) 