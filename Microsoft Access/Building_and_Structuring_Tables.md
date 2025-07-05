# Building and Structuring Tables in Microsoft Access

This guide explains how to create and structure tables in Microsoft Access, a core task in designing a reliable and efficient database. Tables serve as the foundation for all other Access components.

---

## Understanding Table Design

Tables are made up of fields (columns) and records (rows). Each field holds a specific type of data (text, number, date, etc.), and each record contains a unique set of values.

---

## Creating Tables

### Using Datasheet View
1. Click "Create" > "Table."
2. Enter field names directly into the header row.
3. Use the default AutoNumber for primary key or right-click to set your own.

### Using Design View
1. Click "Create" > "Table Design."
2. Define field names, select data types, and provide descriptions if needed.
3. Set a Primary Key to ensure each record is unique.
4. Save the table with a descriptive name (e.g., `Orders`, `Projects`).

---

## Field Data Types (Common)

| Field Type   | Description                          |
|--------------|--------------------------------------|
| Short Text   | Up to 255 characters                 |
| Long Text    | For longer paragraphs or notes       |
| Number       | For numeric calculations             |
| Currency     | For financial values                 |
| Date/Time    | For scheduling or date tracking      |
| Yes/No       | Boolean values (true/false)          |
| Lookup       | Dropdown based on a list or query    |

---

## Primary Keys and Indexing

- The **Primary Key** uniquely identifies each record.
- Set this on a field like `CustomerID` or `InvoiceNumber`.
- Use **Indexes** to improve query speed but avoid over-indexing.

---

## Best Practices

- Use consistent naming conventions (e.g., CamelCase: `FirstName`, `OrderDate`).
- Avoid special characters or spaces in field names.
- Do not store calculated values—calculate them with queries.
- Normalize your data where possible to avoid redundancy.

---

Structuring your tables effectively is crucial for accurate data entry, efficient queries, and scalable database design. Continue to the next guide to learn about database relationships and normalization.
