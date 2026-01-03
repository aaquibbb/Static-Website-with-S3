# ☁️ Automated Static Website Deployment with AWS S3 & Terraform

## 📖 Project Overview
This project demonstrates the deployment of a static website on **Amazon S3** using **Terraform** as an Infrastructure as Code (IaC) tool. 
Instead of manually configuring buckets and policies via the AWS Console, this project automates the entire lifecycle: from provisioning the storage and handling public access security to uploading the HTML assets automatically.

### 🎯 Key Features
* **Infrastructure as Code:** Fully automated provisioning using Terraform.
* **Dynamic Naming:** Implements `random_id` to ensure globally unique bucket names.
* **Security Automation:** Programmatically handles `block_public_access` settings and Bucket Policies.
* **Asset Management:** Uploads `index.html` and `error.html` objects directly via Terraform with correct MIME types (`content_type = "text/html"`).

---

## 🛠️ Tech Stack
* **Cloud Provider:** AWS (S3)
* **IaC:** Terraform (HCL)
* **Version Control:** Git

---

## 🚀 How to Run This Project

### Prerequisites
* [Terraform](https://developer.hashicorp.com/terraform/downloads) installed (v1.5+).
* [AWS CLI](https://aws.amazon.com/cli/) installed and configured with valid credentials (`aws configure`).

### Steps

```bash
### Step 1: Clone the Repository
git clone https://github.com/aaquibbb/Static-Website-with-S3.git
cd Static-Website-with-S3

### Step 2: Initialise Terraform
terraform init

### Step 3: Plan the Deployment
terraform plan

### Step 4: Apply the Configuration
terraform apply

### Step 5: Access the Website
Apply complete! Resources: 6 added, 0 changed, 0 destroyed.
```
Copy and paste this URL that you get into your browser to view the static site.


## 🗑️ Clean Up
To avoid incurring unnecessary costs on AWS, destroy the resources when you are done testing.
```bash
### Last step: Destroy all the infra
terraform destroy
```
## 🔗 Connect with Me
LinkedIn: https://www.linkedin.com/in/aaquibparvez/

Medium Article: https://medium.com/@aaquib.parvez07/terraform-vs-the-console-why-i-automate-even-simple-s3-websites-a5976ab3c46b
