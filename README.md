# CICD-Corporate-DevOps-Pipeline-Project

Architecture Flow
![image](https://github.com/rogerbarrow/CICD-Corporate-DevOps-Pipeline-Project/assets/46138186/3c3c4ba5-7424-4f8c-af77-aae0fd5fd3b6)


# Phases 1
Set up a Private network environment To keep all our  Application and data private and secure 
* -private
* -Isolated
* -Secure 

# Create a k8 Cluster
Create VM in a secure network 
* Nexus Server
* SonarCube Server
* Jenkins
* Monitoring tool

# Phases 2
Create a 
*Private Git Rep to push Code 

# Phases 3
Create a CI/CD Pipeline

# Step 1 Create a VPC in AWS
![image](https://github.com/rogerbarrow/CICD-Corporate-DevOps-Pipeline-Project/assets/46138186/5e5687e7-0dde-4f58-8dc0-5e38c52de53a)
* Update the Security Group with the correct Ports to define how accessible it will be from outside 
![image](https://github.com/rogerbarrow/CICD-Corporate-DevOps-Pipeline-Project/assets/46138186/2405f1d3-5233-4b2d-ac6e-acc0551d3c93)

# create 3 VM for Kubernetes Cluster
![image](https://github.com/rogerbarrow/CICD-Corporate-DevOps-Pipeline-Project/assets/46138186/35a390c0-29ad-459c-b749-6e2c84390675)

# SSH into all 3 VM
![image](https://github.com/rogerbarrow/CICD-Corporate-DevOps-Pipeline-Project/assets/46138186/6f90d4a7-0060-499e-8cd5-ab5e56714fa4)
![image](https://github.com/rogerbarrow/CICD-Corporate-DevOps-Pipeline-Project/assets/46138186/3a35915f-0c6c-4746-b9d2-734c0d5e894c)

![image](https://github.com/rogerbarrow/CICD-Corporate-DevOps-Pipeline-Project/assets/46138186/90125b8a-4e5a-4400-9baf-93a9aa0ff6b0)
 * run cmmd sudo apt-get update
 * sudo apt install docker.io -y
 * sudo chmod 666 /var/run/docker.sock
 * sudo apt-get install -y apt-transport-https ca-certificates curl gpg
 * Sudo mkdir -p -m 755 /etc/apt/keyrings
* curl -fsSL https://pkgs.k8s.io/core://stable:/v1.28/deb/Release.key | sudo gpg --dearmor -o /etc/apt/keyrings/kubernetes-apt-keyring.gpg
