# 📄 Business Analyst – Middleware Portfolio

This repository contains sample artifacts and documents that demonstrate my work as a **Business Analyst – Middleware**, including API requirement documents, error handling, SLAs, logging definitions, and SQL queries used to drive middleware development.

---

## 🎯 Purpose

- Centralize key BA deliverables for middleware projects  
- Showcase requirements gathering, documentation, and validation  
- Provide reference for developers, QA, and stakeholders  

---

## 💼 My Role & Deliverables

As a Middleware Business Analyst, I am responsible for:

- **Requirements Gathering**  
  Interviewing stakeholders to capture business rules and use cases.  

- **API Specification**  
  Designing endpoints, payloads, authentication, error handling, and SLAs.  

- **Technical Documentation**  
  Writing comprehensive API spec documents and SQL query logic.  

- **Collaboration**  
  Working with developers to translate specs into working services.  

- **Validation & Testing**  
  Ensuring middleware meets business requirements through sample requests and query results.

---

## 📑 Example: Prepayment Calculation API

#### 1. Business Requirements
- Customer Service needs to validate and retrieve prepayment amounts for an agreement number.  
- Replaces the manual “Print Trial Prepayment Calculation” in Confins.  
- Aggregates Outstanding Principal, Principal Due, Interest Due, LC Installment, and Termination Penalty for a given date (must be ≥ today).  
- Supports ongoing maintenance by Application Support.

#### 2. Request Parameters

| Field        | Type    | Required | Rules                                        |
| ------------ | ------- | -------- | -------------------------------------------- |
| `input_id`   | string  | Yes      | Max 20 chars, alphanumeric (AgreementNo or ApplicationID) |
| `value_date` | date    | Yes      | `YYYY-MM-DD`, must be ≥ today                |

> For the full API specification—including endpoints, response examples, error codes, SLAs, logging, and SQL queries—see  
> 🔗 [Business Analyst Middleware File List](https://github.com/anugrahrio/Business-Analyst-Middleware-File-List)
