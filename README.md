# EnverSoft Software Developer Assessment

This repository includes the solutions for the Software Developer Interview assessment:

- **Mini Project**: Supplier Management Web Application
- **Exercise 1**: Array Comparison
- **Exercise 2**: CSV File Processor

---

## 📂 Projects Overview

| Project        | Description |
|----------------|-------------|
| [Supplier Portal Client](https://github.com/Nkosinathi-dev1/supplier-portal-client) | Angular frontend for managing suppliers (Mini Project) |
| [Supplier Portal Server](https://github.com/Nkosinathi-dev1/supplier-portal-server) | .NET 9 Web API backend for supplier data management (Mini Project) |
| [Exercise 1](https://github.com/Nkosinathi-dev1/exercise1) | C# Console App comparing two integer lists |
| [Exercise 2](https://github.com/Nkosinathi-dev1/CsvDataProcessor) | C# CSV Processor that outputs sorted names and addresses |

---

## 🖥️ Mini Project: Supplier Portal

![Supplier Management Portal](https://github.com/user-attachments/assets/f657eab5-2560-4d99-8eea-d2391a0a0739)



### Client

- Repository: [Supplier Portal Client](https://github.com/Nkosinathi-dev1/supplier-portal-client)
- Framework: Angular 17
- Development Server:
  - Run `ng serve`
  - Open `http://localhost:4200/`
- **Backend API URL:** `https://localhost:7158`
- Features:
  - Add new suppliers (company name and phone number)
  - Search suppliers by company name

### Server

- Repository: [Supplier Portal Server](https://github.com/Nkosinathi-dev1/supplier-portal-server)
- Framework: .NET 9 Web API
- Database: MS SQL Server

### 🛠️ Setup Instructions (Server)

1. **Navigate** to the `supplier-portal-server` project folder.  
2. Choose **one** of the two options below:

| Option | Creates DB | Creates table | Seeds data | Command |
|--------|------------|---------------|------------|---------|
| **A – EF Core** | ✅ | ✅ (via migrations) | ❌ | `dotnet ef database update` |
| **B – SQL scripts** | ✅ | ✅ | ✅ | See **Option B** panel |

<details>
<summary>Option B — Run SQL scripts manually</summary>
📄 Script files

| What it does | File |
|--------------|------|
| Create DB only | [`create_supplier_db.sql`](https://github.com/Nkosinathi-dev1/supplier-portal-server/blob/master/create_supplier_db.sql) |
| Seed data only | [`seed_suppliers.sql`](https://github.com/Nkosinathi-dev1/supplier-portal-server/blob/master/seed_suppliers.sql) |
| Create **and** seed (one-shot) | [`create_supplier_db_and_seed_suppliers.sql`](https://github.com/Nkosinathi-dev1/supplier-portal-server/blob/master/create_supplier_db_and_seed_suppliers.sql) |

### ▶️ Quick usage

**All-in-one**

```sql
:r supplier-portal-server/scripts/create_supplier_db_and_seed_suppliers.sql
```
</details>  

> **Note**:  
> The database consists of only **one table** (`Suppliers`) as required for the proof of concept.

### Architecture

- **Three-tier architecture**: 
  - Presentation Layer (Angular)
  - Services Layer (.NET 9 Web API)
  - Data Layer (EF Core with MS SQL)

---

## 🧩 Exercise 1: Array Comparison

- Repository: [Exercise 1](https://github.com/Nkosinathi-dev1/exercise1)
- Description:
  - Find common elements between two integer arrays.
  - Find elements unique to each array.
- Technology: C# Console Application.

---

## 📄 Exercise 2: CSV File Processor

- Repository: [CsvDataProcessor](https://github.com/Nkosinathi-dev1/CsvDataProcessor)
- Description:
  - Read a CSV file.
  - Output two text files:
    1. First and last name frequencies, sorted by frequency descending and then alphabetically.
    2. Addresses sorted by street name alphabetically.
- Includes:
  - Unit tests using xUnit.

---

## 🚀 How to Run

- Make sure you have **Node.js**, **Angular CLI**, **.NET 9 SDK**, and **SQL Server** installed.
- Clone each repository.
- Follow the setup instructions provided in each project folder.

---

## 📬 Contact

> **Developer:** Nkosinathi Ngele  
> **Email:** nkosinathi.ngele.dev@gmail.com
> **Phone:** 073 695 4921
---
