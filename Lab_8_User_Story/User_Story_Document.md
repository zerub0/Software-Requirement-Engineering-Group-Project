## User Story Development

**Objective**

To prepare agile user stories and acceptance criteria for the Bus Ticketing System.

**Step 1:** Study Agile Project Requirements

For this lab, we will use the **Bus Ticketing System** requirements gathered from previous labs (Labs 2-5). We will convert those requirements into user stories.

**Step 2:** Write User Stories in Standard Format

2.1 What is a User Story?

A user story is a short, simple description of a feature told from the perspective of the user. The standard format is:

"As a [type of user], I want [some goal] so that [some reason]."

2.2 User Stories for Bus Ticketing System

Here are the user stories organized by actor:

**Passenger User Stories**

| **ID** | **User Story** | **Priority** |
|--------|----------------|--------------|
| US-01 | As a **passenger**, I want to **search for bus routes by origin, destination, and date** so that **I can find available buses for my trip**. | High |
| US-02 | As a **passenger**, I want to **view bus schedules** so that **I can plan my travel time**. | High |
| US-03 | As a **passenger**, I want to **select and reserve specific seats** so that **I can secure my preferred seating**. | High |
| US-04 | As a **passenger**, I want to **book tickets online** so that **I don't have to visit the terminal physically**. | High |
| US-05 | As a **passenger**, I want to **make payments using mobile money or cards** so that **I can pay conveniently**. | High |
| US-06 | As a **passenger**, I want to **receive booking confirmations via SMS and email** so that **I have proof of my booking**. | High |

**Bus Operator User Stories**

| **ID** | **User Story** | **Priority** |
|--------|----------------|--------------|
| US-07 | As a **bus operator**, I want to **manage bus schedules** so that **passengers can book available trips**. | High |
| US-08 | As a **bus operator**, I want to **manage bus routes** so that **I can define where buses travel**. | High |
| US-09 | As a **bus operator**, I want to **set and update pricing for routes** so that **I can adjust fares as needed**. | High |
| US-10 | As a **bus operator**, I want to **monitor seat availability in real-time** so that **I know which seats are booked**. | High |
| US-11 | As a **bus operator**, I want to **generate revenue reports** so that **I can track financial performance**. | Medium |

**Other Actors User Stories**

| **ID** | **User Story** | **Priority** |
|--------|----------------|--------------|
| US-12 | As a **bus company owner**, I want to **view revenue reports** so that **I can assess business profitability**. | High |
| US-13 | As an **administrator**, I want to **manage user accounts** so that **I can create, update, or delete user access**. | High |
| US-14 | As a **bus driver**, I want to **view the passenger list for my trip** so that **I know who should be on the bus**. | Medium |
| US-15 | As a **customer support staff**, I want to **process refunds** so that **passengers can get their money back**. | Medium |
| US-16 | As a **customer support staff**, I want to **handle passenger complaints** so that **issues are resolved efficiently**. | Medium |

**Step 2:** Apply INVEST Criteria

**INVEST** = **I**ndependent, **N**egotiable, **V**aluable, **E**stimable, **S**mall, **T**estable

| **User Story** | **I** | **N** | **V** | **E** | **S** | **T** | **Pass?** |
|----------------|-------|-------|-------|-------|-------|-------|-----------|
| US-01: Search Bus Routes | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | Yes |
| US-04: Book Tickets | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | Yes |
| US-07: Manage Schedules | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | Yes |
| US-12: View Revenue Reports | ✔ | ✔ | ✔ | ✔ | ✔ | ✔ | Yes |

**Step 3:** Define Acceptance Criteria

**US-01: Search Bus Routes**

As a passenger, I want to search for bus routes by origin, destination, and date so that I can find available buses for my trip.

- AC-01: Passenger can enter origin, destination, and travel date
- AC-02: System validates search fields (no empty fields, valid date)
- AC-03: System displays matching routes with times and prices
- AC-04: If no routes found, system shows: "No bus routes found"
- AC-05: Search results are displayed within 3 seconds

**US-04: Book Tickets**

As a passenger, I want to book tickets online so that I don't have to visit the terminal physically.

- AC-01: Passenger can select a route and view schedule details
- AC-02: Passenger can select seats from the seating layout
- AC-03: System validates seat availability before booking
- AC-04: System creates a booking record with a unique booking ID

**US-12: View Revenue Reports**

As a bus company owner, I want to view revenue reports so that I can assess business profitability.

- AC-01: Owner can filter reports by date range, route, or bus
- AC-02: Report displays total revenue, bookings, and revenue by route
- AC-03: Report can be exported as PDF or Excel
- AC-04: Report is generated within 5 seconds

**Step 4:** Prioritized Product Backlog

**Must Have**

| **ID** | **User Story** | **Actor** |
|--------|----------------|-----------|
| US-01 | Search Bus Routes | Passenger |
| US-04 | Book Tickets | Passenger |
| US-05 | Make Payments | Passenger |
| US-07 | Manage Schedules | Bus Operator |
| US-08 | Manage Routes | Bus Operator |

**Should Have**

| **ID** | **User Story** | **Actor** |
|--------|----------------|-----------|
| US-06 | Receive Confirmations | Passenger |
| US-10 | Monitor Seat Availability | Bus Operator |
| US-11 | Generate Revenue Reports | Bus Operator |
| US-12 | View Revenue Reports | Bus Company Owner |

**Could Have**

| **ID** | **User Story** | **Actor** |
|--------|----------------|-----------|
| US-15 | Process Refunds | Customer Support |
| US-16 | Handle Complaints | Customer Support |
