# OrangeHRM Final Automation Scope

**Author:** Jyothi Aradhya  
**Project:** OrangeHRM Playwright Automation Framework  
**Document:** Final Automation Scope

## 1. Purpose

This document defines the final scope of the initial OrangeHRM Playwright automation implementation.

The scope is based on the application analysis, module inventory, critical business workflows, test scenario inventory, automation candidate assessment, manual-only assessment, feasibility assessment, and final prioritization performed during the automation strategy phase.

The objective is to establish a focused and measurable automation scope that provides strong regression value while maintaining a practical implementation and maintenance effort.

## 2. Automation Scope Definition

The initial automation implementation will focus on stable, repeatable, business-relevant UI workflows that provide strong regression value.

The project will not attempt to automate every functionality available in OrangeHRM.

The selected scenarios represent the initial automation baseline. Additional scenarios may be added during future framework expansion based on business value, regression requirements, feasibility, and automation ROI.

## 3. In-Scope Modules

| Module | Scope |
|---|---|
| Login / Authentication | Core authentication and logout workflows |
| Dashboard | Dashboard validation after successful login |
| Admin | Selected user management workflows |
| PIM / Employee Management | Core employee management workflows |
| Leave | Core leave request and approval workflows |

## 4. In-Scope Test Scenarios

### 4.1 Login / Authentication

| Test Case ID | Test Scenario |
|---|---|
| TC-LOGIN-001 | Login with valid credentials |
| TC-LOGIN-002 | Login with invalid username |
| TC-LOGIN-003 | Login with invalid password |
| TC-LOGIN-004 | Login with blank username |
| TC-LOGIN-005 | Login with blank password |
| TC-LOGIN-006 | Login with both fields blank |
| TC-LOGIN-007 | Logout from the application |

### 4.2 Dashboard

| Test Case ID | Test Scenario |
|---|---|
| TC-DASH-001 | Verify dashboard is displayed after successful login |

### 4.3 Admin

| Test Case ID | Test Scenario |
|---|---|
| TC-ADMIN-001 | Create a new system user |
| TC-ADMIN-002 | Search for an existing system user |
| TC-ADMIN-003 | Validate required fields while creating a user |

### 4.4 PIM / Employee Management

| Test Case ID | Test Scenario |
|---|---|
| TC-PIM-001 | Add a new employee with valid details |
| TC-PIM-002 | Validate required fields while adding employee |
| TC-PIM-004 | Search for an existing employee |
| TC-PIM-005 | View employee details |
| TC-PIM-006 | Search for a non-existing employee |
| TC-PIM-007 | Update employee information |
| TC-PIM-008 | Validate updated employee information |

### 4.5 Leave

| Test Case ID | Test Scenario |
|---|---|
| TC-LEAVE-001 | Submit a leave request with valid details |
| TC-LEAVE-002 | Validate leave request required fields |
| TC-LEAVE-003 | View submitted leave request |
| TC-LEAVE-004 | Approve a pending leave request |
| TC-LEAVE-005 | Reject a pending leave request |

## 5. Initial Automation Coverage

The initial scope contains **23 test scenarios** across five functional areas.

| Functional Area | Number of Scenarios |
|---|---:|
| Login / Authentication | 7 |
| Dashboard | 1 |
| Admin | 3 |
| PIM / Employee Management | 7 |
| Leave | 5 |
| **Total** | **23** |

## 6. Framework Scope

In addition to implementing the selected test scenarios, the Playwright framework will demonstrate:

- Playwright Test
- TypeScript
- Page Object Model
- Reusable page and component interactions
- Test data management
- Environment and configuration management
- Reusable fixtures where appropriate
- Reliable locators and assertions
- Test tagging and categorization
- Screenshot and trace support
- HTML test reporting
- Parallel execution where appropriate
- Cross-browser execution where appropriate
- Git/GitHub version control
- GitHub Actions CI/CD
- Maintainable test organization
- Smoke and regression test organization

The framework capabilities may evolve as implementation progresses.

## 7. Initial Automation Approach

The automation implementation will follow a structured approach:

1. Establish the Playwright project and execution environment.
2. Establish configuration and test data management.
3. Implement reusable page objects and components.
4. Automate P0 scenarios first.
5. Add selected P1 scenarios according to the approved scope.
6. Organize tests into smoke and regression suites.
7. Implement reporting and execution diagnostics.
8. Integrate the framework with GitHub Actions.
9. Review reliability, maintainability, and automation coverage.
10. Expand the framework only when justified by business and automation value.

## 8. Scope Selection Rationale

The selected scenarios were prioritized because they provide a strong combination of:

- Business criticality
- Regression value
- Execution frequency
- Repeatability
- Predictable outcomes
- Application stability
- Technical feasibility
- Manageable test data requirements
- Reasonable maintenance effort
- Expected automation ROI

The initial scope therefore focuses on authentication, employee management, administrative user management, and leave-management workflows.

## 9. Future Expansion

The following scenarios are currently outside the initial implementation scope but may be considered for future automation:

| Test Case ID | Test Scenario |
|---|---|
| TC-DASH-002 | Navigate between dashboard menu sections |
| TC-PIM-003 | Add employee with optional details |
| TC-TIME-001 | Access Time/Attendance functionality |
| TC-TIME-002 | Submit a time-related entry |
| TC-REC-001 | Add a recruitment candidate |
| TC-REC-002 | Search for a recruitment candidate |
| TC-MYINFO-001 | View employee personal information |
| TC-MYINFO-002 | Update employee personal information |
| TC-DIR-001 | Search employee using Directory |
| TC-DIR-002 | View employee information from Directory |

Future expansion will be based on business priority, regression needs, technical feasibility, stability, maintenance effort, and automation ROI.

## 10. Scope Change Management

Any addition or removal of automation scenarios will be evaluated against the established automation decision criteria.

Scope changes may be introduced when:

- Business priorities change
- New regression requirements are identified
- Application functionality changes
- A scenario becomes more or less stable
- Test data requirements change
- Automation ROI changes
- Framework capabilities evolve

Significant scope changes will be documented and tracked through version control.

## 11. Scope Boundary

The initial automation scope is intentionally limited to selected OrangeHRM UI workflows.

The existence of functionality outside this scope does not indicate that the functionality is unsuitable for automation.

It indicates that the functionality has been deferred from the initial implementation based on prioritization and project objectives.

## 12. Success of the Initial Scope

The initial automation scope will be considered successful when the selected scenarios can be executed reliably through the Playwright framework and provide meaningful regression coverage while maintaining acceptable execution time, stability, and maintainability.

Detailed success criteria will be defined separately as part of the automation strategy documentation.