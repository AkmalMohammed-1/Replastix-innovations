# ♻️ RePlastix Innovations: Transforming Plastic Waste into Sustainable Solutions

This project implements a customized **Salesforce CRM** solution for RePlastix Innovations – a pioneering organization in **plastic waste collection, recycling, and sustainable product distribution**. The objective is to streamline operations, improve inventory and order tracking, and automate restock notifications with real-time monitoring and Apex logic.

---

## 🚀 Key Features

- **Custom Objects** to manage Plastic Waste, Recycling Centers, Recycled Products, Orders, and Restock Requests
- **Flows & Automation** for low stock alerts, order tracking, and data updates
- **Validation Rules** to enforce clean, consistent data
- **Role-Based Access Control** for Inventory, Sales, and Recycling Teams
- **Apex Triggers & Classes** for:
  - Stock deduction on order placement
  - Restock request creation and fulfillment
  - Email notifications on restock approval
- **Batch Jobs & Scheduled Flows** for inventory monitoring and request generation

---

## 📦 Technologies Used

- **Salesforce Platform**
- **Apex (Object-Oriented Programming Language)**
- **Record-Triggered & Scheduled Flows**
- **Lightning App Builder**
- **Validation Rules**
- **Email Alerts (via Apex Messaging)**
- **Developer Console for Code Implementation**

---

## 🏗️ Custom Objects Overview

| Object Name                                        | Purpose                                          |
|---------------------------------------------------|--------------------------------------------------|
| `Re_Plastic_Innovations_Plastic_Waste__c`         | Tracks collected plastic waste details          |
| `Re_Plastic_Innovations_Recycling_Center__c`      | Manages assigned recycling centers              |
| `Re_Plastic_Innovations_Recycled_Product__c`      | Stores recycled products and stock levels       |
| `Re_Plastic_Innovations_Order__c`                 | Handles customer orders                         |
| `Re_Plastic_Innovations_Restock_Request__c`       | Manages restock requests for low-stock products |

---

## 💻 Project Modules (Apex Components)

1. **InventoryManager.cls**  
   Handles stock reduction after order placement and stock updates after restock approval.

2. **UpdateStockAfterOrder.trigger**  
   Trigger on `Order__c` to process stock reduction.

3. **UpdateStockAfterRestockApproval.trigger**  
   Trigger on `Restock_Request__c` to approve restock and increase inventory.

4. **EmailNotificationHelper.cls**  
   Sends email to warehouse when a restock is approved.

5. **InventoryManagerTest.cls**  
   Apex test class for 100% code coverage of business logic.

---

## 📸 Suggested Screenshots to Include

- Custom App (Lightning App Builder)
- Tabs for each Object (e.g., Waste, Orders, Restock)
- Sample Records for:
  - Plastic Waste entry
  - Recycled Product with stock
  - Order creation triggering stock deduction
  - Restock Request auto-generated
- Flow diagram (Scheduled Flow for Stock Monitoring)
- Email (Mocked screenshot showing restock email)
- Developer Console with Apex Class and Trigger

---

## 📈 Future Scope

- Salesforce Mobile SDK App for warehouse/field team
- Customer Community Portal for order placement and tracking
- WhatsApp/SMS Integration for alerts
- Einstein AI Recommendations for restock and sales patterns
- Custom Reports & Dashboards for real-time insights

---

## 🧑‍💻 Developer

**Name:** Mohammed Abdul Adam Akmal  
**Email:** adamakmal_mohammedabdul@srmap.edu.in  
**Tools:** Salesforce Dev Console, Flow Builder, VS Code (optional)

---

## 📝 License

This project is for educational and demonstration purposes only.
