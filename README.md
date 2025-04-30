# 🏗 SIA – Sistema Integral de Abastecimientos

## 🧭 Overview
**SIA** (Sistema Integral de Abastecimientos) is a multi-module enterprise Windows application developed in **C#** and **SQL Server**, designed to unify and modernize multiple legacy systems under one platform at AHMSA.  
Created during a company-wide resource reorganization, the system centralized operations for the **Purchases**, **Warehouse**, and **Projects** departments.  

It was built as a modular Windows Forms system featuring a Ribbon-style interface, screen embedding, and shared architecture with **[SICAP](https://github.com/HermiloOrtega/SICAP)** and other internal tools.

## 💡 Idea & Concept
The goal of SIA was to migrate scattered tools, spreadsheets, and outdated software into a single, role-based system that:
- Enabled cross-department workflow visibility
- Standardized procurement and warehouse operations
- Enabled administrators to track petty cash and material testing
- Allowed future extensibility for new departments or modules

## ✨ Features & Functionality
- 🔒 Secure Login with 3-attempt limit and session tracking
- 🖥 Environment selection (DEV/QAS/PRD)
- 🚫 Multi-instance prevention and resolution auto-restart
- 📊 RibbonBar UI with embedded module screens (parent/child)
- 🔧 Admin tools to:
  - Lock access per module
  - Force update sessions
  - View system version, broadcast messages, or close user sessions
- 🧾 Action logging: Tracks when users open screens, save data, or perform workflow steps

## ⚙️ Tech Stack
- **Language:** C#
- **Framework:** .NET WinForms
- **Database:** SQL Server
- **IDE:** Visual Studio
- **Reporting:** Crystal Reports
- **Infrastructure:** Windows Servers with network-based deployments

## 🏗 Architecture & Design
- Ribbon-style multi-module system with embedded form loading
- Single executable with role-based access management
- Modular structure per direction (Warehouse, Projects, Purchasing)
- Shared DB architecture with **[SICAP](https://github.com/HermiloOrtega/SICAP)** and other systems
- Configurable deployment per environment (DEV/QAS/PRD)

## 🚀 Installation & Setup
- **Prerequisites:** .NET Framework, SQL Server, permissions for shared folder
- **Startup Behavior:** Launch at boot, restricts multiple instances
- **Access Control:** Centralized through internal user table

> **Note:** Installation is handled by internal IT and system admin for access provisioning.

## 🧑‍💻 Usage
1. Login and select environment
2. Navigate using Ribbon menu
3. Access modules like Material Testing or Petty Cash
4. Save actions are logged; drilldowns available per module
5. Admins can restrict features or push updates

## 🔍 My Role & Contributions
- 💼 Architect and full-stack developer for the core SIA platform
- 🧱 Designed and developed the database, UI, and logic from scratch
- 🔧 Integrated admin control tools for update safety
- 🤝 Led collaboration across 3 departments after staff reorganization

## 🧗 Challenges & Learnings
- Migrated fragmented tools to a cohesive structure
- Integrated cross-department logic for budgeting, stock, and contracts
- Created self-updating features and session fallback logic
- Managed user expectations and continuous improvement post-launch

## 📈 Future Enhancements
- Add more cross-department KPIs
- Web version migration for external access
- Integrate advanced reporting and analytics tools

## 🪪 License
⚠️ **Internal Use Only**  
Originally published under MIT; changed to **CC BY-NC-ND 4.0** as of April 22, 2025.

## 🔗 Related Projects
- [SIA – Petty Cash Module](#)
- [SIA – Material Testing Module](#)