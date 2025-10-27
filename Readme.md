HNG DevOps Stage 2 - Blue/Green Deployment with Nginx Failover

This project implements a Blue/Green deployment pattern using Nginx as a reverse proxy and failover controller.  
It ensures zero-downtime by automatically switching traffic to the Green instance when the Blue instance fails.


## ⚙️ Components

| Service | Description | Port |
|----------|--------------|------|
| nginx | Reverse proxy + failover handler | 8080 |
| app_blue | Primary Node.js service | 8081 |
| app_green | Backup Node.js service | 8082 |

---

##  How to Run Locally
Clone the repo
bash run the below command
git clone https://github.com/Amazingpanam/hng13-stage2-devops.git
cd hng13-stage2-devops
