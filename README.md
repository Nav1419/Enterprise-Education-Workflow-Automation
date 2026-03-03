# Enterprise Education Resource Automation System (ERAS)

## Overview

The Enterprise Education Resource Automation System (ERAS) is a low-code workflow automation platform designed to streamline education resource planning across multiple operational centres and headquarters.

Developed during an internship collaboration with a Singapore-based educational support organisation, the system replaces fragmented spreadsheet-based processes with structured automation, centralised data management, and real-time reporting.

---

## Business Challenge

Operational processes previously relied on multiple Excel files maintained independently by different centres. This resulted in:

- Manual spreadsheet consolidation  
- High risk of data inconsistency  
- Complex book requirement calculations  
- Delays in allocation and order generation  
- Limited visibility into enrolment and stock planning  

As enrolment volume increased, the need for structured automation and centralised coordination became critical.

---

## Solution Architecture

The system follows a modular three-layer enterprise architecture:

### 1. Input Layer
- Power Apps frontend for authorised users  
- Structured Excel file uploads (Waitlist & Placement files)  
- Template validation and input standardisation  

### 2. Automation & Data Layer
- Power Automate workflows triggered upon file upload  
- Microsoft Dataverse as a centralised structured data store  
- Enrolment comparison logic  
- Aggregation and allocation rules  
- Configurable buffer calculations  

### 3. Output & Reporting Layer
- Supplier-compatible purchase order generation  
- Automated Outlook email notifications  
- Power BI dashboards for operational monitoring  

![System Architecture](documentation/system_architecture.png)

---

## Core Automation Workflows

### 1. Waitlist Comparison Workflow
- Compares latest vs historical enrolment datasets  
- Detects newly formed classes  
- Identifies new student entries  
- Stores structured delta records in Dataverse  

### 2. Book Ordering Calculation Workflow
- Aggregates confirmed placement data  
- Computes class and student counts per programme  
- Applies subject-level and semester-based calculation rules  
- Incorporates configurable buffer quantities  
- Generates projected book requirements  

### 3. Book Allocation & Purchase Order Workflow
- Allocates books to centres based on enrolment demand  
- Aggregates totals by subject and academic level  
- Transforms outputs into supplier-compatible purchase order format  
- Triggers automated email notifications  

![Workflow Overview](documentation/workflow_overview.png)

---

## Dashboard & Reporting

Three Power BI dashboards provide end-to-end visibility:

- Waitlist Monitoring Dashboard  
- Capacity & Planning Dashboard  
- Book Allocation Dashboard  

Interactive filters enable review by programme, subject, centre, and academic level, supporting data-driven operational decisions.

---

## Technology Stack

- Microsoft Power Apps  
- Microsoft Power Automate  
- Microsoft Dataverse  
- Microsoft Power BI  
- Excel Automation  
- Outlook Integration  

---

## Technical Skills Demonstrated

- Enterprise workflow automation design  
- Modular system architecture planning  
- Low-code application development  
- Structured data modelling using Dataverse  
- Rule-based automation implementation  
- Cross-platform integration (Application → Automation → Reporting)  
- Business process optimisation  
- Data validation and traceability design  

---

## Impact

- Reduced manual administrative workload  
- Improved cross-centre data consistency  
- Increased operational visibility  
- Established a scalable foundation for future integration  

---

## Disclaimer

This repository presents a portfolio case study version of the system.  
All organisation-specific details have been generalised.  
No confidential data, internal workflow exports, or proprietary configurations are included.
