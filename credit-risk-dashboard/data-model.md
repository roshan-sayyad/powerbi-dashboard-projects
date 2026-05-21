# Credit Risk Data Model

## Fact Table

### fact_loans
Contains loan-level transactional metrics.

Columns:
- loan_id
- customer_id
- exposure_amount
- default_probability
- risk_grade

---

## Dimension Tables

### dim_customer
Customer demographic information.

### dim_date
Calendar and reporting hierarchy.

### dim_risk_grade
Risk segmentation details.

---

## Relationships

fact_loans.customer_id → dim_customer.customer_id
fact_loans.risk_grade → dim_risk_grade.risk_grade
