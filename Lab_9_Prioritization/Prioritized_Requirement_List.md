# Prioritized Requirement List - Bus Ticketing System

---

## Objective

To analyze and prioritize software requirements for the Bus Ticketing System.

---

## Step 1: Review Gathered Requirements

Review all the requirements gathered from previous labs (Labs 2-5) for the Bus Ticketing System.

### Summary of Requirements

| **Category** | **Examples** |
|--------------|--------------|
| Functional Requirements | FR-01 to FR-08 |
| Non-Functional Requirements | NFR-01 to NFR-05 |
| User Stories | US-01 to US-16 |

---

## Step 2: Conduct Feasibility Analysis

### 2.1 What is Feasibility Analysis?

Feasibility analysis evaluates whether a requirement can be implemented given the project's constraints (technical, economic, legal, operational, and schedule).

### 2.2 Feasibility Analysis Report

| **Requirement** | **Feasibility Status** | **Justification** |
|-----------------|------------------------|-------------------|
| FR-05: Make Payments | Feasible with Constraints | Requires integration with third-party payment gateway and security compliance |
| NFR-02: 99.9% Uptime | Feasible with Constraints | Requires investment in reliable hosting infrastructure and backup systems |
| All Other Requirements | Feasible | Can be implemented with existing technology and available resources |

---

## Step 3: Apply MoSCoW Prioritization

### 3.1 What is MoSCoW?

MoSCoW is a prioritization technique that categorizes requirements into four groups: Must have, Should have, Could have and Won't have.

### 3.2 MoSCoW Prioritization for Bus Ticketing System

#### Must Have (Critical Requirements)

| **ID** | **Requirement** | **Category** | **Justification** |
|--------|-----------------|--------------|-------------------|
| FR-01 | Search Bus Routes | M | Users must be able to find available routes |
| FR-02 | View Schedules | M | Users must see schedule details |
| FR-04 | Book Tickets | M | Core functionality of the system |
| FR-05 | Make Payments | M | Must process payments to complete bookings |
| FR-08 | Manage Schedules | M | Bus operators must manage schedules |
| FR-10 | User Authentication | M | Security and access control |
| NFR-01 | 3-second Response Time | M | Performance expectation for user satisfaction |

#### Should Have (Important Requirements)

| **ID** | **Requirement** | **Category** | **Justification** |
|--------|-----------------|--------------|-------------------|
| FR-03 | Select Seats | S | Enhances user experience but not critical |
| FR-06 | Send Confirmations | S | Important for user confidence |
| FR-07 | Trip Reminders | S | User convenience |
| NFR-02 | 99.9% Uptime | S | Important for reliability but 99.9% is a high bar |
| NFR-04 | Mobile Responsive | S | Important for accessibility |

#### Could Have (Nice to Have Requirements)

| **ID** | **Requirement** | **Category** | **Justification** |
|--------|-----------------|--------------|-------------------|
| NFR-05 | Amharic Language Support | C | Expands accessibility but not critical |
| US-13 | Process Refunds | C | Important but can be manual initially |
| US-16 | Handle Complaints | C | Can be manual initially |

#### Won't Have (Not Included in Current Release)

| **ID** | **Reason** |
|--------|------------|
| Real-time GPS Tracking | Future enhancement |
| Bus Maintenance System | Outside system scope |
| Employee Payroll | Outside system scope |

---

## Step 4: Identify Requirement Conflicts

### 4.1 What is a Requirement Conflict?

A requirement conflict occurs when two or more requirements are incompatible or contradictory.

| **Conflict ID** | **Requirement 1** | **Requirement 2** | **Nature of Conflict** | **Resolution** |
|-----------------|-------------------|-------------------|------------------------|----------------|
| C-01 | NFR-01: Response time within 3 seconds | NFR-05: Amharic language support | Performance vs. Internationalization | Prioritize performance; add language support later |
| C-02 | FR-05: Make Payments | NFR-02: 99.9% Uptime | Payment processing requires high availability | Both are important; use redundant systems for payment |
| C-03 | US-08: Manage Routes | US-14: View Passenger Lists | Route changes may affect driver passenger lists | Implement notification system when routes change |
| C-04 | NFR-02: 99.9% Uptime | Budget Constraints | Cost vs. Reliability | Start with 99.5% uptime; improve incrementally |

---

## Step 5: Document Final Decisions

### 5.1 Final Prioritized Requirement List

| **Priority** | **Category** | **Requirements** |
|--------------|--------------|------------------|
| 1 | Must Have | FR-01, FR-02, FR-04, FR-05, FR-08, FR-10, NFR-01 |
| 2 | Should Have | FR-03, FR-06, FR-07, NFR-02, NFR-04 |
| 3 | Could Have | NFR-05, US-13, US-16 |
| 4 | Won't Have | Real-time GPS, Maintenance System, Payroll |

---

### 5.2 Conflict Resolution Summary

| **Conflict ID** | **Resolution Decision** |
|-----------------|-------------------------|
| C-01 | Implement performance requirements first; add Amharic in future phase |
| C-02 | Implement with a single payment gateway initially; add redundancy later |
| C-03 | Notify drivers when routes change via dashboard notifications |
| C-04 | Start with 99.5% uptime; improve to 99.9% in future phases |

---

### 5.3 Assumptions and Constraints

| **Type** | **Description** |
|----------|-----------------|
| Assumption | Users have access to smartphones or computers with internet |
| Assumption | Payment gateway provider is reliable and secure |
| Assumption | Bus operators are computer literate |
| Constraint | Budget is limited; prioritize essential features |
| Constraint | Timeframe is 6 months for the first release |
| Constraint | Must comply with transport authority regulations |

---

## References

| **Reference** | **Source** |
|---------------|------------|
| Software Requirements Engineering Practical Guidelines Manual (SWEG3104) | Course Document |
| Bus Ticketing System Project Scenario | Lab 2 |
| Functional and Non-Functional Requirements | Lab 4 |
| Software Requirements Specification (SRS) | Lab 5 |
| User Stories and Acceptance Criteria | Lab 8 |
| MoSCoW Prioritization Method | Agile Methodology |
| Feasibility Analysis | Requirements Engineering |
