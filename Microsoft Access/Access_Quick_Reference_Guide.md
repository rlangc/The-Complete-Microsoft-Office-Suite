# Microsoft Access Quick Reference Guide

This quick reference guide provides a concise overview of essential features, shortcuts, and tools in Microsoft Access to support everyday database design, navigation, and productivity.

## Common Keyboard Shortcuts

| Action                          | Shortcut         |
|---------------------------------|------------------|
| Save Object                     | Ctrl + S         |
| Open Object                     | Ctrl + O         |
| Close Object                    | Ctrl + W or Ctrl + F4 |
| Cut                             | Ctrl + X         |
| Copy                            | Ctrl + C         |
| Paste                           | Ctrl + V         |
| Undo                            | Ctrl + Z         |
| Redo                            | Ctrl + Y         |
| Switch Between Views            | F5 (Form), F12 (Save As) |
| Toggle Navigation Pane          | F11              |
| Zoom In/Out in Design View      | Shift + F2       |

## Interface Navigation Map

- **Navigation Pane**: Shows all database objects (Tables, Queries, Forms, Reports, Macros, Modules).
- **Ribbon Tabs**:
  - **Home**: Basic operations like sorting, filtering, and clipboard tools.
  - **Create**: Add tables, queries, forms, reports, and macros.
  - **External Data**: Import/export from Excel, SharePoint, ODBC, etc.
  - **Database Tools**: Relationships, performance analyzer, and macro management.

## Object Types & Purpose

| Object Type | Description |
|-------------|-------------|
| **Tables**  | Store raw data in fields (columns) and records (rows). |
| **Queries** | Retrieve, filter, update, and calculate data from tables. |
| **Forms**   | Provide a user-friendly interface for data input and display. |
| **Reports** | Format and print data summaries and layouts for sharing. |
| **Macros**  | Automate routine actions like opening forms or running reports. |
| **Modules** | Hold custom VBA code for advanced automation and logic. |

## Essential Tools & Features

- **Relationships Tool**:  
  - Found under **Database Tools → Relationships**  
  - Define connections between tables using primary and foreign keys.

- **Compact & Repair**:  
  - Use regularly to reduce file size and fix minor corruption.  
  - Access via **File → Info → Compact & Repair Database**

- **Property Sheet**:  
  - Customize form and control behavior.  
  - Toggle via **Design View → Property Sheet**.

- **Expression Builder**:  
  - Helps create formulas and criteria for fields, controls, and queries.  
  - Access in query criteria row or form controls.

## Field Data Types (Common)

| Data Type      | Use Case Example                 |
|----------------|----------------------------------|
| Short Text     | Names, email addresses           |
| Long Text      | Notes, descriptions              |
| Number         | Quantities, percentages          |
| Currency       | Financial values                 |
| Date/Time      | Scheduling, timestamps           |
| Yes/No         | Boolean flags (true/false)       |
| Lookup Wizard  | Dropdown selection from a list   |

## Tips for Working Smarter

- **Always name fields and objects descriptively** (e.g., `CustomerID`, not `Field1`).
- **Use lookup fields** for consistency in form inputs.
- **Avoid storing calculated values**—calculate on-demand with queries.
- **Split your database** into front-end (forms, queries, reports) and back-end (data tables) for multi-user environments.

#

> Use this guide as a quick reference when building, editing, or troubleshooting Access databases. For deeper guidance, refer to the full Access user documentation in this repository.
