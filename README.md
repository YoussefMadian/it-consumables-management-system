# IT Consumables Management & Release System

This project is an enterprise-ready solution built using **Microsoft Power Platform** to manage IT consumables stock and release transactions efficiently.

---

## 🚀 Overview

The system automates:
- IT consumables stock tracking
- Release transactions logging
- Automatic stock deduction
- Monthly reporting (Stock & Release)

It is designed following ERP and warehouse best practices.

---

## 🧱 Architecture

**Technologies Used:**
- SharePoint Online (Data storage)
- Power Apps (User Interface)
- Power Automate (Business Logic & Automation)
- Outlook (Email Reporting)


---

## 📂 SharePoint Lists

### 1. Consumables (Master Data)
Stores all consumables and stock information.

Key columns:
- Item Name
- Stock
- No of Printers
- To Order
- Oracle Code
- Site

### 2. Consumables_Release (Transactions)
Logs every consumables release.

Key columns:
- Release Date
- Item (Lookup)
- Quantity
- Released To
- Printer
- Location
- Released By

---

## 🔄 Power Automate Flows

### Flow 1 – Stock Update on Release
- Trigger: When a release item is created
- Logic: Stock = Stock – Released Quantity

### Flow 2 – Monthly Stock Status Report
- Trigger: Monthly (Day 1)
- Output: Styled HTML table sent via email

### Flow 3 – Monthly Release Report
- Trigger: Monthly (Day 1)
- Logic: Filter releases for previous month
- Output: Detailed release report via email

---

## 🎨 Email Formatting
- HTML tables with CSS borders
- Clean and management-ready format
- No JSON or raw SharePoint objects

---

## 🔐 Design Principles
- Release records are **final and not editable**
- All stock updates are automated
- Full audit trail through SharePoint

---

## 📸 Screenshots
Screenshots are provided for:
- Power Apps UI
- SharePoint list schemas
- Power Automate flows
- Sample email reports

---

## 📈 Future Enhancements
- Return process
- Low stock alerts
- Power BI dashboards
- ERP / Oracle integration

---

## 👨‍💻 Author
Youssef Madian  
IT Infrastructure Engineer
