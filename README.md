# Retail Banking Customer 360 – Sample Power Apps Package

## Overview

This repository contains a **Power Apps solution package (.zip)** that demonstrates a **Retail Banking Customer 360** experience.

The package is intended for **demo and learning purposes** and showcases how relationship managers or contact center agents can view a unified customer profile, including **credit card and financial information**, within a single Power App.

> ⚠️ **Important**: All financial data used in this sample is **hardcoded** and provided **for demonstration purposes only**.

---

## What This Package Demonstrates

- Retail Banking **Customer 360** user experience  
- Consolidated customer profile view  
- Credit card overview (limits, balances, status)  
- Sample financial KPIs presented in a clean UI  
- Power Apps solution packaging and deployment approach  

---

## Package Contents

The solution package (`.zip`) includes:
- A **Power Apps Canvas App**
- Supporting solution components (if applicable)
- Sample logic using **hardcoded financial data**

---

## Credit Card Data Model

This sample requires configuration of a **Credit Card data model** for the app to function correctly.

### Required Fields (Sample)

Ensure the following fields exist in your environment (Dataverse recommended):

- `CustomerId`
- `CardNumber` (masked)
- `CardType`
- `CreditLimit`
- `OutstandingBalance`
- `AvailableCredit`
- `CardStatus`
- `PaymentDueAmount`
- `PaymentDueDate`

> The app uses **static / hardcoded values** for these fields by default to keep the solution simple and environment-agnostic.

---

## Setup Instructions

### 1. Import the Solution Package

1. Go to **Power Apps** → **Solutions**
2. Select **Import solution**
3. Upload the `.zip` package from this repository
4. Complete the import process

---

### 2. Configure the Credit Card Data Model

- Create or verify the Credit Card table and required fields
- Ensure field names match what the app expects
- Alternatively, review and update local collections used by the app

---

### 3. Update Hardcoded Financial Data

- Open the Canvas App from the imported solution
- Review the `OnStart` or screen `OnVisible` logic
- Update hardcoded customer and credit card values as needed for your demo

---

### 4. Run the App

- Save and publish the app
- Launch it from Power Apps to explore the Customer 360 experience

---

## Intended Use Cases

- Retail banking demos and storytelling  
- Customer 360 UX prototyping  
- Presales and enablement scenarios  
- Internal learning and experimentation  

---

## Non-Goals

This sample does **not** include:
- Live banking or core system integrations  
- Real customer or financial data  
- Security, compliance, or regulatory controls  
- Production-ready architecture  

---

## Disclaimer

This solution is provided **as-is** for demonstration purposes only.

- Do **not** use in production environments  
- Do **not** connect to real customer or financial data  
- No compliance, regulatory, or security guarantees are implied  

---

## Optional Next Enhancements

- Replace hardcoded data with Dataverse or API integrations  
- Add transaction history and spending analytics  
- Introduce role-based experiences (RM vs Contact Center Agent)  
- Embed Copilot or AI-driven insights for customer interactions  
