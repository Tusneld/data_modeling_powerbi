# From Nightmare Messy data to Star Schema

> Transforming 23 messy, disconnected tables into a clean, high-performance Star Schema in Power BI.

This portfolio project documents the end-to-end process of converting a chaotic real-world dataset into a reliable, governed, and performance-optimized analytical model.

---

## Project Overview

A global B2B company generates transactional data across **North America, Europe, and Asia** - including customer orders, invoices, shipments, and marketing campaigns.

The original data environment consisted of **23 messy, disconnected tables** with no clear structure. This project refactors that environment into a professional **Star Schema**, ready for accurate reporting and scalable analytics.

---

## Problem Statement

The starting dataset presented classic enterprise data challenges:

- **No Star Schema** → complex many-to-many relationships
- **Poor data quality** → duplicates, inconsistent naming, and null values
- **Siloed tables** → unreliable reporting and slow performance
- **Lack of governance** → no single source of truth for key metrics

---

## Approach

The transformation followed a structured **four-phase workflow**:

### 1. Preparation
Organized raw data in Power Query using a clear folder structure (`Stage`, `Dimensions`, `Facts`).

### 2. Building Dimensions
Merged, cleaned, and standardized descriptive tables (Customers, Products, Campaigns, etc.) into reusable dimension tables.

### 3. Building Facts
Identified the correct grain of each business process and built core fact tables (Sales, Inventory, Campaigns, Order Fulfillment).

### 4. Refinement & Security
- Created a central **Date Table**
- Implemented core business measures
- Applied **Row Level Security (RLS)** for role-based access

---

## Modeling Standards

To ensure consistency, maintainability, and scalability, the following standards were applied:

| Standard              | Implementation                          |
|-----------------------|-----------------------------------------|
| Naming Convention     | `snake_case` for all tables & columns   |
| Dimension Tables      | Prefixed with `dim_`                    |
| Fact Tables           | Prefixed with `fact_`                   |
| Surrogate Keys        | Suffixed with `_key`                    |
| Schema Design         | Strict Star Schema (no fact-to-fact relationships) |
| Data Minimization     | Removed unnecessary descriptive columns |

---

## Key Outcomes

- **Improved Performance** - Reduced model complexity and faster report responsiveness
- **Higher Data Quality** - Eliminated duplicates, nulls, and inconsistent naming
- **Strong Governance** - Established a single source of truth for business metrics
- **Secure Access** - Implemented Row Level Security for controlled data visibility

---

## Tech Stack

- **Power BI Desktop**
- **Power Query**
- **Excel** (source data – 23 tables)

---

## Project Takeaways

This project demonstrates how to turn a typical “nightmare” data environment into a clean, production-ready analytical model - applying real-world data modeling best practices used in enterprise BI teams.

---

## License

This project is intended for portfolio and educational purposes.
