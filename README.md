# OrangeHRM Playwright Automation Framework

**Author:** Jyothi Aradhya
**Project:** OrangeHRM Playwright Automation Framework
**Status:** Module 0 — Strategy & Planning Completed

---

## 1. Project Overview

This project is a practical **Playwright automation framework for the OrangeHRM web application**, designed using a structured automation engineering approach.

The project focuses not only on writing automated tests, but also on demonstrating how automation candidates are evaluated, prioritized, scoped, designed, implemented, stabilized, and integrated into CI/CD.

The framework is being developed incrementally using **Playwright with TypeScript and Playwright Test**.

The automation strategy follows:

> **Application → Modules → Business Workflows → Test Scenarios → Automation Candidates → Manual-Only Assessment → Feasibility → Prioritization → Final Scope → Implementation**

The goal is to build a maintainable, reliable, reusable, and scalable automation framework rather than simply automating every technically possible scenario.

---

## 2. Application Under Test

**Application:** OrangeHRM

**Application Type:** Web-based Human Resource Management Application

The application provides functional areas such as:

* Login / Authentication
* Dashboard
* Admin
* PIM / Employee Management
* Leave
* Time
* Recruitment
* My Info
* Performance
* Directory
* Maintenance
* Buzz

The project uses OrangeHRM as the Application Under Test (AUT) for demonstrating practical UI automation and framework engineering practices.

---

## 3. Project Objectives

The primary objective is to develop a maintainable Playwright automation framework that provides reliable automated coverage for selected high-value OrangeHRM workflows.

### Business Objectives

* Reduce repetitive manual regression effort
* Provide faster feedback for critical workflows
* Improve regression coverage
* Support release validation
* Enable repeatable test execution
* Detect defects earlier through automated validation

### Quality Objectives

* Provide consistent and repeatable validation
* Validate positive and negative scenarios
* Improve regression confidence
* Maintain traceability between scenarios and automated tests
* Complement manual testing rather than replace it

### Technical Objectives

* Build the framework using Playwright and TypeScript
* Use Playwright Test as the test runner
* Apply Page Object Model and reusable components
* Use reliable locators and assertions
* Implement reusable fixtures and utilities where appropriate
* Maintain structured test data and configuration
* Provide meaningful test organization and categorization
* Capture useful execution diagnostics
* Support scalable execution
* Integrate the framework with GitHub Actions CI/CD

---

## 4. Technology Stack

| Area                   | Technology                                        |
| ---------------------- | ------------------------------------------------- |
| Application Under Test | OrangeHRM                                         |
| Automation Tool        | Playwright                                        |
| Programming Language   | TypeScript                                        |
| Test Runner            | Playwright Test                                   |
| Package Manager        | npm                                               |
| Design Approach        | Page Object Model + Reusable Components/Utilities |
| Version Control        | Git                                               |
| Repository             | GitHub                                            |
| CI/CD                  | GitHub Actions                                    |
| Reporting              | Playwright HTML Report                            |
| Diagnostics            | Screenshots, Trace Viewer, Optional Video         |
| Browsers               | Chromium, Firefox, WebKit                         |

---

## 5. Automation Strategy

Automation decisions in this project are based on **business value and maintainability**, not only technical feasibility.

The evaluation considers:

* Business criticality
* Execution frequency
* Repeatability
* Regression value
* Application stability
* Technical feasibility
* Test data availability
* Maintenance effort
* Implementation effort
* Failure investigation effort
* Automation ROI

A scenario being technically automatable does not automatically mean that it should be automated.

The project therefore follows a deliberate candidate-selection and prioritization process before implementation.

---

## 6. Automation Scope

The initial OrangeHRM test scenario inventory contains:

**33 scenarios**

These scenarios were evaluated and prioritized before defining the initial automation scope.

### Initial Automation Scope

**23 scenarios** are included in the initial automation scope.

The scope covers:

* Login / Authentication
* Dashboard
* Admin
* PIM / Employee Management
* Leave

The initial automation scope focuses on stable, repeatable, business-relevant workflows with strong regression value.

---

## 7. Smoke Suite

The initial smoke suite contains **6 critical scenarios**.

| ID           | Scenario                                          |
| ------------ | ------------------------------------------------- |
| TC-LOGIN-001 | Login with valid credentials                      |
| TC-DASH-001  | Verify dashboard displayed after successful login |
| TC-PIM-001   | Add a new employee with valid details             |
| TC-PIM-004   | Search for existing employee                      |
| TC-PIM-007   | Update employee information                       |
| TC-LEAVE-001 | Submit leave request with valid details           |

The smoke suite is designed to provide a small, fast validation of critical application health.

### Smoke vs P0

P0 represents the highest automation implementation priority.

Smoke represents a smaller set of critical scenarios used for quick application health validation.

Therefore:

> **P0 ≠ Smoke**

The smoke suite is a subset of the approved automation scope.

---

## 8. Regression Suite

The initial regression suite contains all **23 approved automation scenarios**.

The regression scope includes:

### Login / Authentication

* TC-LOGIN-001
* TC-LOGIN-002
* TC-LOGIN-003
* TC-LOGIN-004
* TC-LOGIN-005
* TC-LOGIN-006
* TC-LOGIN-007

### Dashboard

* TC-DASH-001

### Admin

* TC-ADMIN-001
* TC-ADMIN-002
* TC-ADMIN-003

### PIM / Employee Management

* TC-PIM-001
* TC-PIM-002
* TC-PIM-004
* TC-PIM-005
* TC-PIM-006
* TC-PIM-007
* TC-PIM-008

### Leave

* TC-LEAVE-001
* TC-LEAVE-002
* TC-LEAVE-003
* TC-LEAVE-004
* TC-LEAVE-005

The smoke suite is a subset of this regression suite.

---

## 9. Automation Prioritization

The 33 identified scenarios were prioritized into three levels.

### P0 — Must Automate

Core automation and regression foundation.

P0 contains **12 scenarios** covering the most critical workflows.

### P1 — Should Automate

High-value secondary regression coverage.

P1 contains **11 scenarios**.

### P2 — Could Automate Later

Lower initial priority scenarios that may be considered during future framework expansion.

P2 contains **10 scenarios**.

The implementation strategy is:

> **P0 → Framework Stabilization → P1 → P2 Evaluation**

---

## 10. Out-of-Scope for Initial Implementation

The following **10 P2 scenarios** are intentionally excluded from the initial automation implementation:

* TC-DASH-002
* TC-PIM-003
* TC-TIME-001
* TC-TIME-002
* TC-REC-001
* TC-REC-002
* TC-MYINFO-001
* TC-MYINFO-002
* TC-DIR-001
* TC-DIR-002

The following modules are also outside the initial implementation scope:

* Time
* Recruitment
* My Info
* Directory
* Performance
* Maintenance
* Buzz

These scenarios and modules may be reassessed later based on business value, regression need, stability, feasibility, maintenance effort, and ROI.

Being out of scope for automation does **not** mean these areas are excluded from testing. Manual testing remains important for appropriate scenarios.

---

## 11. Framework Design Direction

The framework will be developed with maintainability and scalability as primary considerations.

The planned design includes:

* Page Object Model
* Reusable components
* Reusable utilities
* Playwright fixtures
* Structured test data
* Environment/configuration management
* Reliable locators
* Meaningful assertions
* Test categorization and tagging
* Smoke and regression organization
* Cross-browser execution where appropriate
* Parallel execution where appropriate
* Execution diagnostics
* HTML reporting
* CI/CD integration

The detailed implementation structure will evolve during the subsequent modules.

---

## 12. Reliability Approach

The framework will focus on reliable and maintainable automation by using:

* Stable locator strategies
* Appropriate Playwright auto-waiting and synchronization
* Meaningful assertions
* Avoidance of unnecessary hard waits
* Controlled test data
* Reduced dependency on shared test state
* Reusable framework components
* Clear failure classification
* Screenshots and traces for failed tests
* Appropriate retry strategy where required

The objective is to minimize flaky tests and ensure that failures provide useful diagnostic information.

---

## 13. Reporting and Diagnostics

The project will use **Playwright HTML reporting** for test execution results.

Diagnostic capabilities will include:

* Test execution status
* Failure details
* Error messages
* Screenshots
* Trace Viewer
* Optional video recording
* Environment information

These capabilities are intended to support faster failure investigation and debugging.

---

## 14. CI/CD Direction

The framework is planned for integration with **GitHub Actions**.

The intended CI/CD flow includes:

1. Install project dependencies
2. Configure the execution environment
3. Execute smoke tests for early validation
4. Execute regression tests as required
5. Capture execution results
6. Publish test reports
7. Preserve useful diagnostics
8. Provide clear pipeline success/failure feedback

The CI/CD implementation will be developed in a later module.

---

## 15. Automation ROI

Automation decisions are evaluated using an ROI-based approach.

Automation value is considered against:

* Manual execution effort
* Execution frequency
* Business criticality
* Regression risk
* Reusability
* Implementation effort
* Maintenance effort
* Test data complexity
* Failure investigation effort
* Application stability

The project does not follow the principle of:

> "If it can be automated, it should be automated."

Instead, the focus is:

> **Automate where the expected value justifies the implementation and maintenance cost.**

---

## 16. Documentation

The strategy and planning phase is documented under the `docs/` directory.

### Module 0 — Strategy & Planning

| Document | Description                                     |
| -------- | ----------------------------------------------- |
| D0.1     | Application Overview                            |
| D0.2     | Module Inventory                                |
| D0.3     | Critical Business Workflows                     |
| D0.4     | Test Scenario Inventory                         |
| D0.5     | Automation Candidate Assessment                 |
| D0.6     | Manual-Only and Unsuitable Automation Scenarios |
| D0.7     | Automation Feasibility Assessment               |
| D0.8     | Automation Prioritization                       |
| D0.9     | Final Automation Scope                          |
| D0.10    | Out-of-Scope Automation                         |
| D0.11    | Smoke Suite Definition                          |
| D0.12    | Regression Suite Definition                     |
| D0.13    | Automation Objectives                           |
| D0.14    | Success Criteria                                |

All Module 0 strategy documents have been completed and reviewed.

---

## 17. Project Status

### Completed

* Module 0 — Strategy & Planning
* Application analysis
* Module inventory
* Business workflow identification
* Test scenario inventory
* Automation candidate assessment
* Manual-only assessment
* Feasibility assessment
* Automation prioritization
* Initial automation scope
* Out-of-scope definition
* Smoke suite definition
* Regression suite definition
* Automation objectives
* Success criteria
* Module 0 documentation committed to Git

### Upcoming

The next phase will focus on the actual Playwright framework implementation, including:

* Project setup
* Playwright configuration
* TypeScript configuration
* Test execution
* Locators
* Assertions
* Page Objects
* Fixtures
* Test data
* Reusability
* Reporting
* Debugging
* Cross-browser execution
* Parallel execution
* CI/CD
* Framework stabilization

---

## 18. Repository Structure

Current repository structure:

```text
OrangeHRM-Playwright-Automation/
│
├── docs/
│   ├── 01_Application-Overview.md
│   ├── 02_Module-Inventory.md
│   ├── 03_Critical-Business-Workflows.md
│   ├── 04_Test-Scenario-Inventory.md
│   ├── 05_Automation-Candidate-Assessment.md
│   ├── 06_Manual-Only-and-Unsuitable-Automation-Scenarios.md
│   ├── 07_Automation-Feasibility-Assessment.md
│   ├── 08_Automation-Prioritization.md
│   ├── 09_Final-Automation-Scope.md
│   ├── 10_Out-of-Scope-Automation.md
│   ├── 11_Smoke-Suite-Definition.md
│   ├── 12_Regression-Suite-Definition.md
│   ├── 13_Automation-Objectives.md
│   └── 14_Success-Criteria.md
│
└── README.md
```

> The repository structure will evolve as framework implementation begins.

---

## 19. Development Approach

This project is being developed incrementally.

Each module will follow a structured workflow:

1. Define the objective
2. Learn the required concept
3. Implement the concept
4. Execute and validate
5. Review the implementation
6. Document the outcome
7. Commit changes to Git
8. Push the completed module to GitHub
9. Update the project tracker
10. Move to the next module

This approach is intended to maintain traceability between learning, implementation, documentation, and project milestones.

---

## 20. Project Philosophy

This project demonstrates that effective test automation is not simply about writing scripts.

A maintainable automation solution requires decisions around:

* What should be automated?
* Why should it be automated?
* What value does it provide?
* Is the workflow stable enough?
* Is the test data manageable?
* What is the maintenance cost?
* How will failures be diagnosed?
* How will the tests fit into regression and CI/CD?
* How can the framework scale without becoming difficult to maintain?

The project therefore combines **QA strategy, automation engineering, framework design, maintainability, reliability, and CI/CD practices**.

---

## 21. Author

**Jyothi Aradhya**

QA Lead | Software Testing | Test Automation | API Testing | AI in QA

This repository represents a practical automation engineering project focused on building a structured and maintainable Playwright framework for OrangeHRM.
