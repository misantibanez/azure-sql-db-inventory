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

- **Login to your Azure account** before running the script:
  ```bash
  az login

---

## 🚀 Getting Started
**🔧 1. Clone the repository**

      git clone https://github.com/yourusername/azure-sql-db-inventory.git
      cd azure-sql-db-inventory

**📜 2. Make the script executable**

      chmod +x list-azure-sql-databases.sh
      
**▶️ 3. Run the script**

      ./list-azure-sql-databases.sh

---

## 🖥️ Example Output
    
    Fetching details for Resource Group: my-rg, Server: my-sql-server
    
    Name      Size    Status   ZoneRedundant
    --------  ------  -------  --------------
    db1       S0      Online   False
    db2       P1      Online   True

