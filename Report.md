# DevOps Assignment Report: Debugging and Running a Dockerized Application

---
### Cloud Deployment
-Deployed on AWS Ec2: `http://34.227.92.68/`

## Issues Identified

### 1. Nginx Configuration Issues
- **Multiple Typos in nginx Dockerfile**: Multiple typos were fixed , like "latest" , "nginx" , it should be "daemon off" rather than "daemon of" 
- **Port Exposure**: Incorrect port format in `Dockerfile`, fixed it as port 80 

### 2. Python Application Issues
- **Multiple Typos in python Dockerfile**: Multiple typos were fixed like "app" ,
- - **Package Installation**: Typo in package name `netifaces`
- **Command Syntax**: Incorrect Python execution command , it should be  ["python", "app.py"]
 - **Port Exposure**: Incorrect port format in `Dockerfile`, fixed it as port 8000
 -  
### 3. Docker Compose Issues
- **Port Mapping**: Invalid port format (`"eighty:80"`)
- **Network Configuration**: Typo in bridge driver name
- **Volume Mounting**: Incorrect configuration file path

### Screenshots
![Docker container running locally](https://github.com/user-attachments/assets/53341ee6-7baf-4508-8879-f2b9437d62c7)
![Docker container running on ec2 instance](https://github.com/user-attachments/assets/d6aa3004-f934-40c0-a002-5a67142895dc)




---




