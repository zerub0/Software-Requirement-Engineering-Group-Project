# Revised Requirement Document - Bus Ticketing System

---

## Objective

To document revised requirements after validation and verification.

---

## Revised Functional Requirements

| **ID** | **Functional Requirement** |
|--------|----------------------------|
| FR-01 | The system shall allow passengers to search for bus routes by origin, destination, and date of travel. |
| FR-02 | The system shall allow passengers to view available bus schedules with departure and arrival times. |
| FR-03 | The system shall allow passengers to select and reserve specific seats from a seating layout. |
| FR-04 | The system shall allow passengers to book tickets online. |
| **FR-05** | **The system shall allow passengers to make payments using mobile money (Telebirr, M-Pesa) and credit/debit cards.** |
| FR-06 | The system shall send booking confirmations via SMS and email. |
| **FR-07** | **The system shall send trip reminders to passengers 24 hours before departure via SMS and email.** |
| FR-08 | The system shall allow bus operators to add, update, and delete bus schedules. |
| FR-09 | The system shall allow bus operators to generate revenue reports. |
| FR-10 | The system shall authenticate users before allowing access. |

---

## Revised Non-Functional Requirements

| **ID** | **Non-Functional Requirement** |
|--------|--------------------------------|
| NFR-01 | The system shall respond to search queries within 3 seconds. |
| **NFR-02** | **The system shall be available 99.5% of the time for the initial release, with a target of 99.9% in future phases.** |
| NFR-03 | The system shall support at least 1,000 concurrent users. |
| NFR-04 | The system shall be accessible on both web browsers and mobile devices (Android and iOS). |
| NFR-05 | The system shall be available in both English and Amharic languages. |

---

## Revision Summary

| **Requirement** | **Revision Type** | **Description** |
|-----------------|-------------------|-----------------|
| FR-05 | Clarified | Added specific payment methods |
| NFR-02 | Modified | Changed from 99.9% to 99.5% for initial release |
| FR-07 | Completed | Added specific timing and delivery methods |

---

## References

| **Reference** | **Source** |
|---------------|------------|
| Software Requirements Engineering Practical Guidelines Manual (SWEG3104) | Course Document |
| Bus Ticketing System Requirements | Labs 2-5 |
| Review Checklist | Lab 10 |
| Validation Report | Lab 10 |
| Revised Requirement Document | Lab 10 |
