# 🚀 Automated EC2 Instance Provisioning using AWS CLI & Bash

## 📌 Project Overview

This project demonstrates **Infrastructure Automation** by provisioning Amazon EC2 instances using a **Bash script** integrated with **AWS CLI**.
The script ensures **secure, repeatable, and reliable instance creation** by:

* Checking & installing AWS CLI if missing
* Automating EC2 instance launch with user-defined parameters
* Monitoring until the instance reaches the **running state**
* Configuring **VPC subnets, security groups, and key pairs**

---

## 🛠️ Tech Stack

* **Bash** – Automation scripting
* **AWS CLI v2** – Command-line interface for AWS
* **Amazon EC2** – Virtual servers in the cloud
* **VPC & Subnets** – Networking and isolation
* **Security Groups** – Firewall rules
* **IAM** – Secure access control

---

## 📂 Project Structure

```
.
├── create_ec2_instance.sh   # Main script to create EC2 instance
└── README.md                # Project documentation
```

---

## ⚙️ Prerequisites

Before running the script, ensure you have:

* **AWS account** with proper permissions (EC2, IAM, VPC access)
* **AWS CLI configured** with credentials:

  ```bash
  aws configure
  ```
* **Bash shell** (Linux/macOS, or WSL on Windows)

---

## 🚀 Usage

1. **Clone the repository**

   ```bash
   git clone https://github.com/VENKATESH-KATTAMURI/shell-scripting.git
   cd shell-scripting
   ```

2. **Make the script executable**

   ```bash
   chmod +x create_ec2_instance.sh
   ```

3. **Run the script**

   ```bash
   ./create_ec2_instance.sh
   ```

4. **Script parameters to update (inside the script):**

   ```bash
   AMI_ID="ami-xxxxxxxx"
   INSTANCE_TYPE="t2.micro"
   KEY_NAME="your-key"
   SUBNET_ID="subnet-xxxxxxxx"
   SECURITY_GROUP_IDS="sg-xxxxxxxx"
   INSTANCE_NAME="Shell-Script-EC2-Demo"
   ```

---

## 📊 Workflow

1. **Check & install AWS CLI** (if not already installed)
2. **Provision EC2 instance** using AWS CLI
3. **Tag the instance** for identification
4. **Monitor instance state** until it becomes `running`
5. **Secure instance** with key pairs, VPC subnets, and security groups

---

## ✅ Example Output

```
Creating EC2 instance...
Instance i-0abc12345def67890 created successfully.
Waiting for instance i-0abc12345def67890 to be in running state...
Instance i-0abc12345def67890 is now running.
EC2 instance creation completed.
```

---

## 📖 Learning Outcomes

* Hands-on experience with **AWS CLI & Bash scripting**
* Automated EC2 provisioning using **Infrastructure-as-Code** principles
* Improved knowledge of **VPC networking, IAM, and Security Groups**
* Built a **reusable DevOps utility** for AWS

---

Would you like me to also **add a system architecture diagram (VPC → Subnet → Security Group → EC2)** in markdown (with a link to an image you can upload), so recruiters see a visual workflow too?
