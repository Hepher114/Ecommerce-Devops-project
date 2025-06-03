This project demonstrates the end-to-end implementation of a cloud-native, microservices-based e-commerce application using AWS, Kubernetes, Terraform, and GitOps. Below are the key technical components covered:

1. AWS Infrastructure & Security
AWS account setup and IAM role/policy configuration.

EC2 instance deployment with security group rules (inbound/outbound traffic).

2. Containerization & Local Deployment
Docker installation and microservice containerization.

Local environment setup using Docker Compose.

Building, running, and validating containers.

3. Infrastructure as Code (Terraform)
Terraform installation and AWS provider configuration.

State management: Backend setup, locking, and remote statefiles.

Automated provisioning of VPC, EKS cluster, and Kubernetes resources.

4. Kubernetes Orchestration
EKS cluster deployment via Terraform.

Kubernetes manifests for deployments, services, and ingress.

Ingress controller (NGINX) setup with custom domain routing.

Persistent storage: StorageClass, PV, and PVC configuration.

Application validation on Kubernetes.

5. CI/CD & GitOps Automation
GitHub Actions workflow for CI (testing, image builds).

Argo CD installation and configuration for GitOps-driven CD.

End-to-end pipeline: Code commit → CI → Argo CD sync → Production.

6. Custom Domain & DNS (Route 53)
Route 53 hosted zone configuration.

Ingress routing with SSL/TLS termination.