# Understanding Relationships and Normalization in Microsoft Access

This guide covers how to define relationships between tables and apply basic normalization to ensure your database is structured for consistency, accuracy, and scalability.

## What Are Relationships?

Relationships connect tables using keys—usually a **Primary Key** in one table and a **Foreign Key** in another. This creates a structured way for Access to combine data.

### Types of Relationships
- **One-to-One**: Rare; used when data is split between two tables for design or security.
- **One-to-Many**: Most common. One customer can have many orders.
- **Many-to-Many**: Requires a junction table to link records (e.g., Students and Classes).

## Creating Relationships in Access

1. Go to **Database Tools** > **Relationships**.
2. Add relevant tables to the window.
3. Drag the primary key from one table onto the foreign key in the other.
4. Check **Enforce Referential Integrity** for data consistency.
5. Click **Create**.

## What Is Normalization?

Normalization is the process of organizing data to reduce redundancy and dependency.

### Normal Forms
- **1NF**: Eliminate repeating groups; ensure each field contains only atomic values.
- **2NF**: Remove partial dependencies on a composite primary key.
- **3NF**: Eliminate fields not dependent on the primary key.

## When to De-normalize

- In reporting scenarios where performance is prioritized.
- When read-heavy operations outweigh update-heavy operations.

## Best Practices

- Start with an Entity-Relationship Diagram (ERD).
- Use descriptive field names that clarify table relationships.
- Always define primary keys and use foreign keys where appropriate.

A well-normalized database with clearly defined relationships ensures reliable data and efficient queries. Continue to the next guide to start designing forms for clean and user-friendly data entry.
