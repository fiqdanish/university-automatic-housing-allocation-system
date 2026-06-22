# SysDataVerse — Enterprise Architecture & Room Allocation Engine

An enterprise architecture analysis and design project for **Universiti Tun Hussein Onn Malaysia (UTHM)**, including the design and low-code implementation of a **Room Allocation Engine** sub-system for hostel management.

---

## 📖 Overview

UTHM has migrated most of its academic, administrative, and support systems to a new platform, but the systems remain only partially integrated. This causes duplicated data, inconsistent workflows, and slower service delivery. This project applies **Enterprise Architecture (EA)** principles to analyze the current landscape, propose an improved architecture, and demonstrate the value through a focused, working sub-system.

## ❗ Problem Statement

- Independent and partially integrated systems lead to **data stored in multiple places**, **inconsistent workflows**, and **slower service delivery**.
- UTHM's strategic ICT goals (stronger infrastructure, integrated applications, workforce development) are hard to achieve **without a structured EA approach**.
- The lack of architectural alignment makes it difficult to ensure all systems work together coherently.

## 🎯 Objectives

1. **Analyze** the existing information systems at UTHM that support key university operations (academic management, teaching & learning, administrative processes, and student services).
2. **Design** an enterprise-level system architecture using EA principles and structured system design methodologies.
3. **Propose & demonstrate** a well-aligned architecture through the implementation of a representative sub-system (the Room Allocation Engine).

## 📦 Scope

**In-Scope**
- Enterprise Architecture analysis (AS-IS and TO-BE) for UTHM.
- Design and low-code implementation of the **Room Allocation Engine** sub-system.
- System modelling: Use Case, Activity, Sequence, ERD, and Class diagrams.
- Interface design and core allocation/conflict-resolution logic.

**Out-of-Scope**
- Full university-wide system migration.
- Integration with all external/legacy UTHM systems.
- Production deployment and live data.

---

## 🏗️ System Design

| Artifact | Description |
|---|---|
| **EA AS-IS** | Current enterprise architecture of UTHM |
| **EA TO-BE** | Proposed, integrated enterprise architecture |
| **System Architecture** | Hostel Management System architecture |
| **Use Case Diagram** | Room Allocation Engine actors & use cases |
| **Activity Diagrams** | UC-001 to UC-008 process flows |
| **Sequence Diagrams** | UC-001 to UC-008 interaction flows |
| **ERD** | Database design (Applications, Room, Rules, College, allocationInfo) |
| **Class Diagram** | Object-oriented structure of the engine |

### Core Use Cases

| ID | Use Case | Actor |
|---|---|---|
| UC-001 | Configure Allocation Rules | Admin |
| UC-002 | Modify Room Assignment | Admin |
| UC-003 | Check Room Availability | Admin & Engine |
| UC-004 | Check for Allocation Conflict | Admin |
| UC-005 | Resolve Conflict | Admin |
| UC-006 | Auto-allocate Room | Engine |
| UC-007 | Update Room Status | Admin & Engine |

---

## 🛠️ Technology Stack

- **SAP Build** — Low-code / no-code platform for rapid application development.
- **SAP Analytics Cloud** — Data visualization, reporting, and Business Intelligence (BI).
- **Lucidchart** — Enterprise architecture and UML diagramming.
- **GitHub** — Version control and project management / progress tracking.

---

## 📂 Repository Structure

```
.
├── Articles/ # Reference papers (EA in higher education)
├── Diagrams/
│ ├── Activity/ # Activity diagrams (UC-001 … UC-008)
│ ├── Sequence/ # Sequence diagrams (UC-001 … UC-008)
│ ├── Use Case/ # Use case diagram
│ ├── Class diagram.jpeg
│ └── ERD.png
├── EA/
│ ├── EA as-is.png
│ ├── EA to-be.png
│ ├── EA Presentation (SysDataverse).pdf
├── SysDataVerse_AfiqDanish.pdf # Full project report
├── Room Allocation Engine.pdf # Engine design document
└── README.md
```

---

## 🧩 Room Allocation Engine — Key Features

- **Configurable allocation rules** (gender, year of study, room capacity).
- **Automatic room allocation** based on predefined rules.
- **Conflict detection** for duplicate assignments and overcapacity.
- **Manual override** to modify or reassign student rooms.
- **Real-time room status & availability** tracking.

---

## 💭 Reflection

**Context.** UTHM's partially integrated systems cause duplicated data, inconsistent workflows, and slower service — making a structured EA approach genuinely worthwhile.

**Approach.** Analyzed the existing landscape, mapped AS-IS and TO-BE architectures, then scoped down to the Room Allocation Engine — modelled thoroughly before building it on SAP Build with SAP Analytics Cloud for BI.

**What worked / what didn't.** The modelling-first discipline made the low-code build far smoother, and strong team collaboration kept the report organized and on schedule. Harder parts were getting the auto-allocation and conflict-checking logic right within low-code constraints, and bridging the broad EA vision with a single implementable sub-system.

**What I'd do differently.** Narrow scope earlier and validate the allocation rules and data model up front — treating each system as part of a larger, well-aligned enterprise architecture rather than building in isolation.


---

## 📄 License

Academic project for SECP3744, UTM. For educational and reference purposes.
