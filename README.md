# 📊 Data Anonymisation Pipeline  
## Excel Project #2 — Commonwealth Bank Virtual Experience Program  

This project focuses on designing and implementing a privacy pipeline to anonymise sensitive customer data while preserving its analytical value for downstream data science applications.  

As part of a simulated business engagement between Commonwealth Bank and InsightSpark, the objective was to prepare customer mobile app data for secure sharing by removing or transforming personally identifiable information (PII) and reducing the risk of linkage attacks.

---

## Business Problem  

Before customer data can be used for analytics, machine learning, or business intelligence initiatives, sensitive information must be protected.  

The challenge was to anonymise the dataset in a way that:

- Protects customer privacy
- Prevents re-identification
- Minimises linkage attack risks
- Preserves useful business insights

---

## Dataset  

**Source File:** `mobile_customers.csv`

The dataset contains customer records from users who signed up for the mobile app over a three-year period.

Sensitive attributes included:

- Customer names
- Phone numbers
- Passport numbers
- Credit card details
- Date of birth
- Income information
- Geographic data

---

## Project Objectives  

- Research data anonymisation techniques
- Identify direct and indirect identifiers
- Design a privacy transformation pipeline
- Preserve analytical usefulness
- Export a secure anonymised dataset

---

## Anonymisation Techniques Applied  

### 1. Column Suppression  
Removed fields with no analytical value:

- Names
- Passport numbers
- Credit card numbers

### 2. Data Masking  
Masked identifying information.

Example:

```text
0412345678 → 04******78
```

### 3. Generalisation  
Converted exact values into ranges.

| Original | Anonymised |
|----------|------------|
| Age: 27 | 25–34 |
| Income: $72,400 | $50K–$75K |

### 4. Date Transformation  

```text
1998-04-15 → 1998
```

### 5. Geographic Aggregation  

```text
Sydney CBD → New South Wales
```

---

## Tools Used  

- Microsoft Excel
- CSV File Processing
- Data Validation
- Privacy Preservation Techniques

---

## Skills Demonstrated  

- Data Privacy
- Data Cleaning
- Data Transformation
- Risk Mitigation
- Spreadsheet Analytics
- Business Intelligence

---

## Deliverables  

```bash
├── mobile_customers.csv
├── mobile_customers_anonymised.csv
├── anonymisation_workbook.xlsx
└── README.md
```

---

## Outcome  

Successfully created an anonymised customer dataset that protects sensitive customer information while maintaining valuable analytical insights for future data science initiatives.
