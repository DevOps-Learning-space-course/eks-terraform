### Prerequisites

- [AWS CLI](https://aws.amazon.com/cli/)
- [Terraform](https://cloud.google.com/sdk/docs/install)

### Additional resources

- If you use VSCode, hover over variables to see the description/type in .tf and .tfvars files with the [Terraform extension](https://marketplace.visualstudio.com/items?itemName=HashiCorp.terraform).
- [Official module documentation]()
- [How to setup awsci and terraform](https://learn.hashicorp.com/tutorials/terraform/aws-build)

#### AWS CLI Cheat Sheet

```bash
# Obtain account
aws sts get-caller-identity
# Obtain username and userarn
aws iam get-user
# Obtain rolearn
aws iam list-roles
# Obtain groups
aws iam list-groups
```

---

### Set up a managed kubernetes cluster on EKS

- Navigate into the `eks` directory
- Copy `terraform.tfvars.example` file to `terraform.tfvars` file and fill in missing configuration parameters
- Open a terminal and run the following:

```bash
cd aws/eks # if you haven't done so already
# Initializes the directory
terraform init
# Sets up the EKS cluster
terraform apply


