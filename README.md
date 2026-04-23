# Operational & Financial Performance Audit of a Private Clinic
### Power BI • SQL Server • Data Modeling • DAX

---

## Project Overview

This project simulates a real consulting mission for a private clinic that lacked visibility on its operational inefficiencies and financial performance.

Although data existed in the system (appointments, billing, pharmacy, expenses), management had no clear answers to critical questions such as:

- Why are many appointments not happening?
- Is long patient waiting time caused by doctors or scheduling?
- Where is revenue really coming from?
- Where is money being wasted?
- Is the clinic truly profitable?

This project transforms raw data into a **decision-support dashboard** designed for the clinic director.

---

## Business Questions Answered

The dashboard answers the questions that matter to management:

1. Why are almost 1 in 4 appointments lost (no-shows and cancellations)?
2. Which doctors and services are responsible for the highest revenue losses?
3. Is waiting time a doctor issue or a system scheduling issue?
4. Does the clinic earn more from medical services or from the pharmacy?
5. Where does the clinic spend most of its money?
6. What is the real net profit after all expenses?
7. Which operational actions would recover the most money?

---

## Data Sources & Modeling

Data was extracted, cleaned, and modeled from multiple tables:

- Appointments
- Doctors
- Services
- Billing (payments)
- Pharmacy sales
- Expenses

A **star schema** was designed in Power BI to ensure accurate calculations and cross-analysis between operational and financial data.

---

## Key Metrics Discovered

| Metric | Value | Industry Benchmark | Verdict |

| No-show rate | **9.6%** | 3–5% | 🔴 Critical |
| Cancellation rate | **14.5%** | <8% | 🔴 Critical |
| Average waiting time | **47 min** | 15–20 min | 🔴 Critical |
| Revenue lost from missed appointments | **1.07M MAD / year** | — | 🔴 Major leakage |
| Pharmacy share of total revenue | **53%** | 20–30% | 🟡 Risky dependency |
| Profit margin | **17.5%** | 25–35% | 🟡 Below optimal |

---

## Major Insights from the Analysis

### 1️ Waiting time is a system issue, not a doctor issue
All doctors show nearly identical waiting times (~47 minutes), indicating a scheduling problem rather than individual performance.

### 2️ Appointment management is the biggest financial problem
Nearly 25% of appointment value is lost due to no-shows and cancellations, representing more than **1 million MAD** in lost revenue.

### 3️ Certain services drive most of the financial loss
*Petite Chirurgie* alone represents a large portion of lost revenue, making it a priority for operational review.

### 4️ The clinic behaves more like a pharmacy business
Pharmacy sales generate more revenue than medical services, creating a risky business dependency.

### 5️ October is the only loss-making month
This anomaly suggests operational or staffing issues worth investigating.

---

## Business Recommendations

Based on the data findings:

- Implement SMS/WhatsApp appointment confirmations → potential recovery of **1M MAD/year**
- Redesign scheduling process to reduce waiting time by up to 50%
- Audit *Petite Chirurgie* workflow to reduce financial leakage
- Rebalance focus between medical services and pharmacy dependency
- Investigate October anomaly to prevent future losses

---

## Tools & Skills Demonstrated

- SQL Server for data preparation
- Data cleaning and transformation
- Star schema data modeling
- Advanced DAX measures for KPIs
- Power BI dashboard design for executives
- Analytical storytelling and business interpretation

---

## Dashboard Pages

1. **Patient Flow & Appointment Efficiency**
2. **Revenue Lost from Cancellations & No-Shows**
3. **Expenses, Pharmacy Revenue & Net Profit**

---

##  Dashboard Preview

### Patient Flow & Appointment Efficiency
**Overview:**
Analyzes 8,000 appointments to evaluate doctor workload, waiting time, and scheduling efficiency.

**Key Findings:**

1 in 4 appointments is wasted (24% no-show/cancel)
Waiting time (~47 min) is the same for all doctors → scheduling system issue, not doctor performance
Certain services (Echo, Diabétique tests) create longer delays
Appointment demand is uneven across days and services

**Insight:**
The clinic’s main problem is poor scheduling and capacity planning.

<img width="1316" height="695" alt="page1 png" src="https://github.com/user-attachments/assets/cfc45df1-e456-4d05-a920-6d264b73e6ae" />


### Revenue Lost from Cancellations & No-Shows
**Overview:**
Measures the financial impact of missed appointments by linking status with service prices.

**Key Findings:**

1.07M MAD lost due to missed appointments
Petite Chirurgie & Radiologie cause the highest losses
Some months show higher appointment failure rates

**Insight:**
Simple appointment confirmation processes could recover significant revenue.

<img width="1282" height="725" alt="page2 png" src="https://github.com/user-attachments/assets/25226687-9ea4-418e-a880-413d3c6ec11a" />



### Expenses, Pharmacy & Net Profit
**Overview:**
Evaluates where revenue comes from, where money is spent, and the clinic’s real profitability.

**Key Findings:**

Pharmacy generates more revenue than medical services
Expenses consume a large portion of revenue
Profit margin is 17.5% (below optimal for clinics)

**Insight:**
The clinic is profitable but financially unbalanced and overly dependent on pharmacy sales.
<img width="1396" height="732" alt="page3 png" src="https://github.com/user-attachments/assets/7b1f3eba-a550-491f-9b29-15efa8e3c1f8" />


---

## Outcome

This project demonstrates how data can be used not just for reporting, but for:

> **Operational diagnosis, financial auditing, and decision-making support**

[clinic_performance.zip.zip](https://github.com/user-attachments/files/26948987/clinic_performance.zip.zip)



