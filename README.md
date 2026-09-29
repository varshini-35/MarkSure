# MarkSure ⚖️

### Digital Type-Evaluation & Compliance Platform for OIML R-76 Weighing Instruments

MarkSure is an end-to-end digital metrology evaluation and test-report generation platform for **Non-Automatic Weighing Instruments (NAWI)** such as electronic weighing scales, platform scales and other weighing instruments used in trade and industry.

Built around **OIML R 76-1**, MarkSure digitizes the evaluation workflow from instrument registration and test observations to deterministic metrology calculations, compliance analysis, technical review, standardized report generation, report integrity verification and instrument-wise historical tracking.

---

## 🎯 Problem

NAWI type evaluation involves multiple tests, observations, calculations, compliance checks and detailed reporting.

When these activities depend on spreadsheets, manual calculations and separate document templates, the process can become fragmented and repetitive. It can also make report consistency, result verification, revision tracking and historical retrieval more difficult.

MarkSure brings these activities together into a single structured digital workflow.

---

## 💡 Solution

MarkSure connects the complete evaluation lifecycle:

**Instrument → Evaluation → Test Observations → OIML R-76 Calculations → Compliance → Review → Report → Verification → Digital Passport**

The platform combines deterministic metrology calculations with structured workflows, explainable results, evidence traceability and report governance while keeping technical compliance decisions under authorized human review.

---

# 🚀 Key Features

## 1. 🧪 OIML R-76 Metrology Engines

MarkSure provides dedicated calculation and compliance engines for major NAWI evaluation activities, including:

- **Weighing Performance**
  - Automatic Maximum Permissible Error (MPE) evaluation
  - Accuracy-class based evaluation
  - Verification scale interval (`e`) based calculations

- **Repeatability**
  - Multi-series measurement analysis
  - Standard deviation
  - Range evaluation

- **Eccentricity / Corner Load**
  - Evaluation across different loading positions

- **Tare Evaluation**
  - Additive and subtractive tare evaluation
  - Zero-setting behaviour

The calculations are deterministic and rule-driven to ensure reproducible evaluation results.

---

## 2. 🔍 "Show Me Why" — Explainable Compliance

MarkSure does not simply display a PASS or FAIL result.

The platform provides a mathematical explanation connecting:

**Observed Value → Error → Permissible Limit → Applicable Requirement → Compliance Result**

This allows authorized reviewers to understand how a result was obtained and trace it back to the underlying test data.

---

## 3. 📊 "What Changed?" — Report Version Comparison

Finalized reports are preserved through linked versions rather than being silently overwritten.

MarkSure's comparison engine can identify changes across:

- Instrument parameters
- Ambient conditions
- Individual test trials
- Raw calculations
- Compliance results
- Report metadata

The system provides a side-by-side differential view and highlights significant changes, including compliance verdict changes.

---

## 4. 🧪 Rule Impact Simulator

The Rule Impact Simulator provides a controlled regulatory sandbox for testing proposed rule configurations.

Users can create candidate configurations and evaluate their potential impact against historical datasets without modifying the active configuration or original evaluation records.

The simulator can visualize:

- Before/after compliance results
- Pass-rate differences
- Verdict changes
- Potential impact across historical evaluations

Simulation outputs are clearly separated from official evaluation records.

---

## 5. 🪪 Digital Instrument Passport

Each instrument can have a connected digital lifecycle record containing information such as:

- Instrument details
- Evaluation history
- Calibration-related information
- Pattern approval information
- Verification status
- Associated reports
- Relevant events

This provides an instrument-wise historical view rather than treating each report as an isolated document.

---

## 6. 🔐 Report Integrity Verification

Finalized reports can be associated with a **SHA-256 cryptographic integrity hash**.

QR-based verification can be used to access the corresponding verification mechanism and check whether an issued report has been modified after finalization.

This provides a tamper-evident integrity mechanism for digitally issued reports.

---

## 7. 📎 Evidence & Traceability

Supporting evidence such as photographs, documents, test setup information and notes can be associated with relevant evaluations and tests.

This helps establish a traceability chain between:

**Evidence → Test → Observation → Calculation → Compliance Result → Report**

---

## 8. 👥 Role-Based Evaluation Workflow

MarkSure supports role-based access for different participants in the evaluation lifecycle.

### Testing Officer

- Create instruments
- Initiate evaluations
- Enter test observations
- Perform tests
- Attach evidence
- Create and submit reports

### Reviewing Officer

- Review evaluations
- Verify observations
- Inspect calculations
- Review supporting evidence
- Approve or return evaluations
- Finalize reports and revisions

### Administrator

- Manage system-level functions
- Manage laboratories
- Manage rule configurations
- Access audit and oversight functionality

---

## 9. 📄 Automated Report Generation

MarkSure automatically generates structured test reports from verified evaluation data.

Reports can include:

- Instrument information
- Laboratory information
- Test conditions
- Test observations
- Calculations
- Compliance results
- Evidence
- Reviewer information
- Evaluation/report identifiers
- Rule/configuration information

The platform supports PDF and editable report generation to reduce repetitive document preparation.

---

## 10. 🗂️ Repository & Historical Tracking

Completed evaluations and reports are maintained in a centralized repository.

Records can be searched and retrieved using relevant parameters such as:

- Manufacturer
- Model
- Serial number
- Instrument type
- Accuracy class
- Evaluation ID
- Report ID
- Date
- Officer
- Result

This enables instrument-wise historical tracking and faster retrieval of previous evaluations.

---

## 11. 🧾 Audit Trail & Versioning

MarkSure maintains a traceable history of important evaluation and reporting activities.

Report revisions are linked to their previous versions, while relevant actions and timestamps can be retained for audit purposes.

This helps preserve the evolution of an evaluation and its associated reports.

---

# 🔄 End-to-End Workflow

```text
Instrument Registration
        ↓
Evaluation Creation
        ↓
Test Conditions
        ↓
Test Observations
        ↓
OIML R-76 Calculations
        ↓
Validation & Compliance
        ↓
Evidence & Review
        ↓
Report Generation
        ↓
Integrity Verification
        ↓
Repository & Digital Passport
        ↓
Audit & Historical Tracking
```
---
# 🛠️ Tech Stack

| Layer | Technologies |
|---|---|
| **Frontend** | React, TypeScript, Vite, Tailwind CSS, React Router, Recharts, Lucide Icons |
| **State & Resilience** | IndexedDB for continuous form-state persistence and recovery |
| **Backend** | Node.js, Express, TypeScript, REST APIs |
| **Authentication** | JWT, Role-Based Access Control (Testing Officer, Reviewing Officer, Admin) |
| **Database** | PostgreSQL, Prisma ORM |
| **Local Development** | SQLite with Prisma |
| **Calculation Engine** | Deterministic, versioned OIML R-76 rule and calculation engine |
| **Document Generation** | PDFKit, DOCX generation |
| **Report Formats** | Indian / RRSL and OIML CS templates |
| **Security & Integrity** | SHA-256 hashing, QR-based report verification, audit trail |
| **File Handling** | Multer |
| **Deployment** | Netlify, Render, Neon PostgreSQL |
---

# 🌐 Live Application

### MarkSure Web Application

**[https://markksuree.netlify.app/](https://markksuree.netlify.app/)**

### Backend API

**[https://marksure-backend.onrender.com/](https://marksure-backend.onrender.com/)**

---
# 🔑 Demo Login Credentials

Use the following accounts to explore MarkSure's role-based workflow.

| Role | Email | Password |
|---|---|---|
| **Testing Officer** | `officer.test@marksure.gov.in` | `Pass@123` |
| **Reviewing Officer** | `officer.review@marksure.gov.in` | `Pass@123` |
| **Admin** | `admin@marksure.gov.in` | `Pass@123` |

### Role Overview

- **Testing Officer** — Creates evaluations, enters test observations, uploads evidence and submits evaluations for review.
- **Reviewing Officer** — Reviews submitted evaluations, verifies calculations/evidence and approves or returns them for correction.
- **Admin** — Manages the overall system, users and administrative functions.

> **Note:** These credentials are provided for demonstration purposes only.

---

# 🏗️ System Architecture

MarkSure follows a modular full-stack architecture connecting the user interface, evaluation workflow, OIML R-76 calculation engine, reporting layer, security services and database.

```text
                         USERS
                           │
                           ▼
                ┌────────────────────┐
                │ MarkSure Frontend  │
                │ React + TypeScript │
                │ Vite + Tailwind    │
                └─────────┬──────────┘
                          │
                       REST APIs
                          │
                          ▼
                ┌────────────────────┐
                │ MarkSure Backend   │
                │ Node + Express     │
                │ TypeScript         │
                └─────────┬──────────┘
                          │
        ┌─────────────────┼─────────────────┐
        │                 │                 │
        ▼                 ▼                 ▼
 ┌──────────────┐  ┌──────────────┐  ┌────────────────┐
 │ Authentication│  │ Evaluation   │  │ OIML R-76      │
 │ & RBAC       │  │ & Test Mgmt  │  │ Rule Engine    │
 │              │  │              │  │                │
 │ JWT          │  │ Instruments  │  │ Calculations   │
 │ Role Access  │  │ Tests        │  │ Validation     │
 └──────────────┘  │ Observations │  │ Compliance     │
                   │ Evidence     │  │ Applicability  │
                   └──────────────┘  └────────────────┘
                          │
        ┌─────────────────┼─────────────────┐
        │                 │                 │
        ▼                 ▼                 ▼
 ┌──────────────┐  ┌──────────────┐  ┌────────────────┐
 │ Report       │  │ Integrity &  │  │ Governance &   │
 │ Generation   │  │ Verification │  │ Versioning     │
 │              │  │              │  │                │
 │ PDF          │  │ SHA-256      │  │ Audit Trail    │
 │ DOCX         │  │ QR Verify    │  │ Report Versions│
 │ Templates    │  │              │  │ Rule Versions  │
 └──────────────┘  └──────────────┘  └────────────────┘
                          │
                          ▼
                ┌────────────────────┐
                │ PostgreSQL         │
                │ + Prisma ORM       │
                └────────────────────┘
```
---

## 📜 License

This project is licensed under the MIT License.
