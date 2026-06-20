# Validation Report - Bus Ticketing System

---

## Objective

To validate and verify requirement quality for the Bus Ticketing System.

---

## Review Summary

| **Aspect** | **Result** |
|------------|------------|
| Total Requirements Reviewed | 15 |
| Defects Found | 3 |
| Defects Resolved | 3 |
| Requirements Validated | 15 |
| Validation Status | **PASSED** |

---

## Defects Identified

| **Defect ID** | **Requirement** | **Defect Type** | **Severity** | **Status** |
|---------------|-----------------|-----------------|--------------|------------|
| D-01 | FR-05: Make Payments | Ambiguity | High | Resolved |
| D-02 | NFR-02: 99.9% Uptime | Measurability | Medium | Resolved |
| D-03 | FR-07: Trip Reminders | Incompleteness | Low | Resolved |

---

## Review Findings

| **Requirement ID** | **Issue Found** | **Type** | **Suggested Fix** |
|--------------------|-----------------|----------|-------------------|
| FR-05 | Payment method unclear | Ambiguity | Specify exact payment methods (mobile money, card) |
| NFR-02 | "99.9% uptime" may be too costly | Feasibility | Consider 99.5% for initial release |
| FR-07 | Reminder timing not specified | Incompleteness | Specify "24 hours before departure" |

---

## Revised Requirements

| **Original Requirement** | **Revised Requirement** |
|--------------------------|-------------------------|
| FR-05: The system shall allow passengers to make payments. | FR-05: The system shall allow passengers to make payments using mobile money (Telebirr, M-Pesa) and credit/debit cards. |
| NFR-02: The system shall be available 99.9% of the time. | NFR-02: The system shall be available 99.5% of the time for the initial release, with a target of 99.9% in future phases. |
| FR-07: The system shall send trip reminders. | FR-07: The system shall send trip reminders to passengers 24 hours before departure via SMS and email. |

---

## Validation Conclusion

| **Aspect** | **Status** |
|------------|------------|
| All requirements reviewed | ✅ |
| All defects resolved | ✅ |
| Requirements validated | ✅ |
| Validation Status | **PASSED** |

---

## References

| **Reference** | **Source** |
|---------------|------------|
| Software Requirements Engineering Practical Guidelines Manual (SWEG3104) | Course Document |
| Bus Ticketing System Requirements | Labs 2-5 |
| Review Checklist | Lab 10 |
| Validation Report | Lab 10 |
