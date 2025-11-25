GitOps Workflow using ArgoCD on Kubernetes 

Introduction  
This project showcases the creation of a Kubernetes cluster using Kind on an AWS EC2 instance and the deployment of a multi-service Voting Application using Argo CD. It demonstrates modern DevOps practices such as GitOps, automated deployments, cluster orchestration, and application scaling, all within a cloud-hosted environment.

Abstract
The objective of this project is to implement a fully automated deployment pipeline using Kubernetes and Argo CD. The work includes provisioning an EC2 instance, installing Docker and Kind, creating a Kubernetes cluster, and configuring Argo CD for GitOps-based deployments. A cloud-native Voting Application consisting of a Python frontend, Redis, .NET worker, PostgreSQL database, and Node.js results application is deployed using Argo CD. The project highlights reliability, scalability, and efficiency in deploying distributed applications.

Tools Used
•	AWS EC2 – Cloud infrastructure for hosting the Kubernetes cluster
•	Docker – Container runtime for application components
•	Kind – Tool to create local Kubernetes clusters using Docker
•	kubectl – CLI for managing Kubernetes clusters
•	Kubernetes Dashboard – Web interface for cluster visualization
•	Argo CD – GitOps continuous delivery tool
•	GitHub – Repository for manifests and application code


Steps Involved in Building the Project
1. Launching AWS EC2 Instance
A Ubuntu-based EC2 instance was created with necessary security groups and SSH access. The instance served as the host machine for Docker and the Kind Kubernetes cluster.
2. Installing Docker
Docker was installed and configured to run containers required for Kind and the Voting App components.
3. Setting Up Kind Kubernetes Cluster
Kind was installed to create a single-node Kubernetes cluster. The cluster configuration was verified using kubectl.


4. Installing kubectl
The Kubernetes CLI tool was set up to manage and interact with the cluster. Cluster nodes, pods, and services were validated.
5. Configuring Kubernetes Dashboard
The Kubernetes Dashboard was deployed for a visual management interface, allowing easy monitoring of pods, nodes, and deployments.
6. Installing and Configuring Argo CD
Argo CD was installed inside the cluster. The UI was accessed using port forwarding, and admin credentials were configured.
7. Connecting GitHub Repository
A GitHub repository containing deployment YAML files was linked to Argo CD. GitOps workflows were configured to automate syncing and deployments.
8. Deploying the Voting Application
The Voting App, consisting of:
•	Python frontend
•	Redis (vote collector)
•	.NET worker (background processor)
•	PostgreSQL database
•	Node.js results app
was deployed through Argo CD using declarative Kubernetes manifests.
9. Monitoring Deployments and Scaling
Argo CD and the Kubernetes Dashboard were used to monitor rollouts, logs, pod scaling, and resource utilization.

Conclusion
The project successfully demonstrates the implementation of a GitOps-based CI/CD workflow using Kubernetes and Argo CD. Deploying the cloud-native Voting Application validated the benefits of automation, scalability, and reliability. This setup ensures streamlined deployments, improved efficiency, and simplified management of distributed applications on AWS EC2. The system achieved stable performance with high availability and smooth rollouts.



