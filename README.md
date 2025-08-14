# -Monitor-System-Resources-Using-Netdata12
# Task 7: Monitor System Resources Using Netdata

## **Objective**
Install and run **Netdata** to monitor system and application performance metrics in real time.

---

## **Tools Used**
- **Netdata** (Free, open-source monitoring tool)
- **Docker**

---

## **Setup & Installation**

### **1. Run Netdata using Docker**
```bash
docker run -d \
  --name=netdata \
  -p 19999:19999 \
  --cap-add SYS_PTRACE \
  --security-opt apparmor=unconfined \
  netdata/netdata
