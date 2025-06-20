# 🧠 Blue Prism: Automated Data Entry Bot

This repository contains the full documentation and process design for an **Automated Data Entry Bot** built using **Blue Prism v7.4.0**. The bot reads customer data from an Excel file and simulates entering it into a digital form. It was created as a portfolio-ready automation for job applications in banking and financial institutions.

---

## 📌 Project Overview

The goal of this automation is to streamline data entry by automating the process of retrieving customer information from an Excel sheet and simulating manual form inputs.

Key capabilities include:
- Opening and reading Excel files using MS Excel VBO
- Looping through rows of data to extract and simulate input
- Modular design with separate logic for name, email, and phone entry
- Designed with extensibility and scalability in mind

---

## 🧰 Tools & Technologies

- **Platform:** Blue Prism v7.4.0  
- **Objects Used:** MS Excel VBO  
- **Modules:** Process Studio, Data Items, Looping, and Action Blocks  
- **Project Type:** Desktop RPA / Simulation  

---

## 🔄 Process Flow

1. **Start**
2. **Open Workbook** – Uses `MS Excel VBO - Open Workbook`
3. **Read Worksheet** – Converts the sheet into a Collection using `Get Worksheet As Collection`
4. **Loop** through each row in `CustomerDataCollection`:
   - Simulate Name Entry
   - Simulate Email Entry
   - Simulate Phone Entry
5. **End**

All records from the file `CustomerData.xlsx` are processed row by row.

---

## 📂 Project Structure

```text
/BluePrism-AutomatedDataEntryBot
│
├── Process Studio Main Page
│   └── Main workflow design (Start → Loop → Simulated Actions → End)
│
├── Business Objects
│   └── MS Excel VBO (used for reading spreadsheet)
│
├── Data Items
│   └── ExcelFilePath, CurrentName, CurrentEmail, CurrentPhone
│   └── CustomerDataCollection
│
├── Screenshots
│   └── Dashboard (Workforce, Automations, Queues)
│   └── Process Studio Logic
│   └── Version History (Creation, Modifications)
