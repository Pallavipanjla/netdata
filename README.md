# netdata
# 🖥 Task 7: Monitor System Resources Using Netdata

## 🎯 Objective
The goal of this task is to install and run Netdata using Docker to monitor system and application performance metrics in real time.

---

## 🧰 Tools Used
- **Netdata** – Real-time monitoring dashboard (open-source)
- **Docker** – Container runtime to deploy Netdata quickly

---

## 📝 Steps to Complete the Task

### ✅ 1. Install Docker
- Download and install Docker Desktop from: https://www.docker.com/products/docker-desktop
- Verify installation by running:
  ```powershell
  docker --version
 
### ✅ 2. Run Netdata in Docker
docker run -d --name=netdata -p 19999:19999 --cap-add=SYS_PTRACE -v netdataconfig:/etc/netdata -v netdatalib:/var/lib/netdata -v netdatacache:/var/cache/netdata -v "C:/Users/Pallavi:/host" netdata/netdata

### ✅ 3. Access the Netdata Dashboard
http://localhost:19999
---
