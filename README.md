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

### Step 1: Clone the Repository
```bash
git clone [https://github.com/aaquibbb/Static-Website-with-S3.git](https://github.com/aaquibbb/Static-Website-with-S3.git)
cd Static-Website-with-S3
