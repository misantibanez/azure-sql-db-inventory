# 🔍 Azure SQL Database Inventory Script

This Bash script leverages the Azure CLI and `jq` to inventory all **Azure SQL Databases** in your subscription. It organizes the databases by **SQL server** and **resource group**, and displays useful details such as service tier, current status, and zone redundancy.

Ideal for cloud administrators, DevOps engineers, or developers managing large-scale Azure environments.

---

## 📋 Features

- ✅ Lists all Azure SQL Databases across your subscription
- 🗂️ Groups databases by their parent SQL server and resource group
- 📊 Displays database service tier, status, and zone redundancy in a clean table format
- 🔁 Uses only standard CLI tools — no Azure policies or premium features required
- 🧩 Easily customizable for filtering, CSV export, or integration into CI/CD pipelines

---

## 📦 Prerequisites

To use this script, you'll need the following installed:

- **Azure CLI**  
  [Install instructions](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli)
  
- **jq** (Command-line JSON processor)  
  [Install instructions](https://stedolan.github.io/jq/)

- **Login to your Azure account** before running the script:
  ```bash
  az login
