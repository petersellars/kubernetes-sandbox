# Kubernetes Cloud Cluster
Create a Kubernetes cluster in the cloud based on best practice

Provision a Kubernetes cluster with [Terraform](https://www.terraform.io) and [CoreOS](https://coreos.com/) on AWS. The provisioning mimics the original documentation: [Manual Installation](https://coreos.com/kubernetes/docs/latest/getting-started.html) as close as possible.

## Setup

* create a file: `terraform.tfvars`

```
# aws
access_key = "<access key>"
secret_key = "<secret key>"

ssh_public_key = "<ssh public key>"
ssh_private_key_path = "<path to private key file>"

# generate new discovery url: https://discovery.etcd.io/new?size=<master_count>
discovery_url = "<discovery url>"

# cluster
master_count = 1
worker_count = 1
```
