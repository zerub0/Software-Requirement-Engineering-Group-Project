# Conflict Resolution Report - Bus Ticketing System

---

## Objective

To identify and resolve conflicts between requirements for the Bus Ticketing System.

---

## What is a Requirement Conflict?

A requirement conflict occurs when two or more requirements are incompatible or contradictory. Conflicts can arise due to:

- **Technical conflicts** - Requirements that cannot be implemented together
- **Resource conflicts** - Requirements competing for limited resources
- **Schedule conflicts** - Requirements with conflicting timelines
- **Stakeholder conflicts** - Different stakeholders with opposing needs
- **Quality conflicts** - Requirements that trade off against each other (e.g., performance vs. features)

---

## Identified Conflicts

### Conflict C-01: Performance vs. Internationalization

| **Aspect** | **Details** |
|------------|-------------|
| **Requirement 1** | NFR-01: Response time within 3 seconds |
| **Requirement 2** | NFR-05: Amharic language support |
| **Nature of Conflict** | Adding Amharic language support may increase page load times and server response times |
| **Impact** | Users may experience slower response times if both requirements are implemented together |
| **Stakeholders Affected** | Passengers, Bus Operators |

**Resolution:**

| **Decision** | **Justification** |
|--------------|-------------------|
| Prioritize performance (NFR-01) first; add Amharic language support (NFR-05) in a future phase | Performance is critical for user satisfaction; language support is a value-add feature that can be delayed |

---

### Conflict C-02: Payment Processing vs. High Availability

| **Aspect** | **Details** |
|------------|-------------|
| **Requirement 1** | FR-05: Make Payments |
| **Requirement 2** | NFR-02: 99.9% Uptime |
| **Nature of Conflict** | Payment processing requires the system to be highly available; implementing 99.9% uptime is costly |
| **Impact** | Budget constraints may limit the ability to achieve 99.9% uptime |
| **Stakeholders Affected** | Passengers, Bus Company Owner |

**Resolution:**

| **Decision** | **Justification** |
|--------------|-------------------|
| Implement with a single payment gateway initially; add redundancy in future phases | Both requirements are important. Start with a reliable payment gateway and improve infrastructure incrementally |

---

### Conflict C-03: Route Changes vs. Passenger Lists

| **Aspect** | **Details** |
|------------|-------------|
| **Requirement 1** | US-08: Manage Routes (Bus Operator) |
| **Requirement 2** | US-14: View Passenger Lists (Bus Driver) |
| **Nature of Conflict** | When a bus operator changes a route, the bus driver's passenger list may become outdated |
| **Impact** | Bus drivers may have incorrect passenger information |
| **Stakeholders Affected** | Bus Operators, Bus Drivers, Passengers |

**Resolution:**

| **Decision** | **Justification** |
|--------------|-------------------|
| Implement a notification system that alerts bus drivers when routes or schedules change | This ensures drivers always have the latest passenger list and minimizes confusion |

---

### Conflict C-04: Reliability vs. Budget Constraints

| **Aspect** | **Details** |
|------------|-------------|
| **Requirement 1** | NFR-02: 99.9% Uptime |
| **Requirement 2** | Budget Constraints (identified in feasibility analysis) |
| **Nature of Conflict** | Achieving 99.9% uptime requires investment in redundant servers, load balancers, and monitoring tools |
| **Impact** | The project may exceed budget if 99.9% uptime is required immediately |
| **Stakeholders Affected** | Bus Company Owner, Project Manager |

**Resolution:**

| **Decision** | **Justification** |
|--------------|-------------------|
| Start with 99.5% uptime; improve to 99.9% in future phases | This balances cost and reliability. Initial uptime of 99.5% is acceptable for the first release |

---

## Conflict Resolution Summary

| **Conflict ID** | **Requirement 1** | **Requirement 2** | **Resolution Decision** |
|-----------------|-------------------|-------------------|-------------------------|
| C-01 | NFR-01: 3-second Response Time | NFR-05: Amharic Language Support | Prioritize performance; add language support in future phase |
| C-02 | FR-05: Make Payments | NFR-02: 99.9% Uptime | Start with single gateway; add redundancy later |
| C-03 | US-08: Manage Routes | US-14: View Passenger Lists | Implement notification system for route changes |
| C-04 | NFR-02: 99.9% Uptime | Budget Constraints | Start with 99.5% uptime; improve incrementally |

---

## Lessons Learned

| **Lesson** | **Description** |
|------------|-----------------|
| Involve all stakeholders early | Conflicts are easier to resolve when all stakeholders are involved from the beginning |
| Establish clear priorities | A clear priority hierarchy helps resolve conflicts quickly |
| Consider trade-offs | Sometimes requirements must be traded off against each other (e.g., cost vs. quality) |
| Document decisions | All conflict resolution decisions should be documented for future reference |

---

## References

| **Reference** | **Source** |
|---------------|------------|
| Software Requirements Engineering Practical Guidelines Manual (SWEG3104) | Course Document |
| Bus Ticketing System Project Scenario | Lab 2 |
| Functional and Non-Functional Requirements | Lab 4 |
| Software Requirements Specification (SRS) | Lab 5 |
| MoSCoW Prioritization Method | Lab 9 |
| Feasibility Analysis Report | Lab 9 |
| Conflict Resolution | Requirements Engineering |
