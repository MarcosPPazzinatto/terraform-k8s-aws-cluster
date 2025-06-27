# Terraform Kubernetes AWS Cluster

This project uses Terraform to provision a minimal Kubernetes cluster on AWS.  
It includes:

- Custom VPC setup
- IAM credentials for cluster access
- EC2 instances to form a simple control plane and nodes
- (Optional) Integration with `kubeadm` or EKS (in future versions)

## Requirements

- Terraform >= 1.5
- AWS CLI configured
- An AWS account with appropriate permissions

## Modules Structure (Planned)
  
 - vpc/ – custom networking setup
 - iam/ – credentials and roles
 - ec2/ – small cluster setup (2-3 nodes)
 - k8s/ – (coming soon) bootstrap Kubernetes using remote-exec or EKS

## Getting Started

# Initialize Terraform
```
terraform init
```

# Preview the resources
```
terraform plan
```

# Apply and create the infrastructure
```
terraform apply
```

## License  
This project is licensed under the MIT License.
