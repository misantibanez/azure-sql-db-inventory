# 🔍 Azure SQL Database Inventory Script

This Bash script leverages the Azure CLI to inventory all **Azure SQL Databases** in your subscription. It organizes the databases by **SQL server** and **resource group**, and displays useful details such as service tier, current status, and zone redundancy.

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

- **✅ Minimum Role Required**
  To run your script successfully, a user needs at least the Reader role at the subscription level plus visibility into the SQL resources.

  Specifically, they need permission to:
  - List Azure resources (for az resource list)
  - List SQL servers and databases (for az sql db list)
---

## 🚀 Getting Started
- **🔧 1. Clone the repository**

      git clone https://github.com/misantibanez/azure-sql-db-inventory.git
      cd azure-sql-db-inventory
    
- **▶️ 2. Run the script**

      cd scripts
      .\list-azure-sql-databases.ps1
      ![image](https://github.com/misantibanez/azure-sql-db-inventory/tree/main/assets/run_script.png)

---

## 🖥️ Example Output
    
    Fetching details for Resource Group:

    ![image](https://github.com/misantibanez/azure-sql-db-inventory/tree/main/assets/output_example.png)

---
## 🔗 References

- [Azure CLI Documentation](https://learn.microsoft.com/en-us/cli/azure/)
- [Install Azure CLI](https://learn.microsoft.com/en-us/cli/azure/install-azure-cli)
- [Azure CLI `az resource list`](https://learn.microsoft.com/en-us/cli/azure/resource#az-resource-list)
- [Azure CLI `az sql db list`](https://learn.microsoft.com/en-us/cli/azure/sql/db#az-sql-db-list)
- [Azure Built-in Roles: Reader](https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles#reader)
- [Azure Built-in Roles: Contributor](https://learn.microsoft.com/en-us/azure/role-based-access-control/built-in-roles#contributor)
- [Azure Role-Based Access Control (RBAC)](https://learn.microsoft.com/en-us/azure/role-based-access-control/overview)

