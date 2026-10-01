# OrangeHRM Automation Feasibility Assessment

**Author:** Jyothi Aradhya  
**Project:** OrangeHRM Playwright Automation Framework  
**Document:** Automation Feasibility Assessment

## 1. Purpose

This document evaluates the feasibility of automating the test scenarios identified during the automation candidate assessment.

The assessment considers technical feasibility, application stability, test data requirements, repeatability, regression value, maintenance effort, and expected automation ROI.

The purpose is to determine which scenarios are practical and valuable for automation before defining the final Playwright automation scope.

## 2. Feasibility Assessment Criteria

Each scenario is evaluated using the following criteria:

| Criteria | Assessment Focus |
|---|---|
| Technical Feasibility | Whether Playwright can reliably automate the scenario |
| Application Stability | Stability of the functionality and UI under test |
| Test Data | Availability and manageability of required test data |
| Repeatability | Ability to execute the scenario consistently and repeatedly |
| Regression Value | Value provided during recurring regression testing |
| Maintenance / ROI | Expected maintenance effort compared with automation benefit |

The following feasibility levels are used:

- **High** – Strong technical and business justification for automation.
- **Medium** – Technically feasible but requires additional consideration regarding data, complexity, value, or maintenance.
- **Low** – Automation may provide limited value or may not be practical under current conditions.

## 3. Scenario Feasibility Matrix

| Test Case ID | Test Scenario | Technical Feasibility | Application Stability | Test Data | Repeatability | Regression Value | Maintenance / ROI | Overall Feasibility |
|---|---|---|---|---|---|---|---|---|
| TC-LOGIN-001 | Login with valid credentials | High | High | High | High | High | High | High |
| TC-LOGIN-002 | Login with invalid username | High | High | High | High | High | High | High |
| TC-LOGIN-003 | Login with invalid password | High | High | High | High | High | High | High |
| TC-LOGIN-004 | Login with blank username | High | High | High | High | High | High | High |
| TC-LOGIN-005 | Login with blank password | High | High | High | High | High | High | High |
| TC-LOGIN-006 | Login with both fields blank | High | High | High | High | Medium | High | High |
| TC-LOGIN-007 | Logout from the application | High | High | High | High | High | High | High |
| TC-DASH-001 | Verify dashboard is displayed after successful login | High | High | High | High | High | High | High |
| TC-DASH-002 | Navigate between dashboard menu sections | High | High | High | Medium | Medium | Medium | Medium |
| TC-ADMIN-001 | Create a new system user | High | High | Medium | High | High | High | High |
| TC-ADMIN-002 | Search for an existing system user | High | High | Medium | High | High | High | High |
| TC-ADMIN-003 | Validate required fields while creating a user | High | High | High | High | Medium | High | High |
| TC-PIM-001 | Add a new employee with valid details | High | High | Medium | High | High | High | High |
| TC-PIM-002 | Validate required fields while adding employee | High | High | High | High | High | High | High |
| TC-PIM-003 | Add employee with optional details | High | High | Medium | Medium | Medium | Medium | Medium |
| TC-PIM-004 | Search for an existing employee | High | High | Medium | High | High | High | High |
| TC-PIM-005 | View employee details | High | High | Medium | High | High | High | High |
| TC-PIM-006 | Search for a non-existing employee | High | High | High | High | Medium | High | High |
| TC-PIM-007 | Update employee information | High | High | Medium | High | High | High | High |
| TC-PIM-008 | Validate updated employee information | High | High | Medium | High | High | High | High |
| TC-LEAVE-001 | Submit a leave request with valid details | High | High | Medium | High | High | High | High |
| TC-LEAVE-002 | Validate leave request required fields | High | High | High | High | High | High | High |
| TC-LEAVE-003 | View submitted leave request | High | High | Medium | High | High | High | High |
| TC-LEAVE-004 | Approve a pending leave request | High | High | Medium | Medium | High | Medium | High |
| TC-LEAVE-005 | Reject a pending leave request | High | High | Medium | Medium | High | Medium | High |
| TC-TIME-001 | Access Time/Attendance functionality | High | High | High | Medium | Medium | Medium | Medium |
| TC-TIME-002 | Submit a time-related entry | High | Medium | Medium | Medium | Medium | Medium | Medium |
| TC-REC-001 | Add a recruitment candidate | High | High | Medium | Medium | Medium | Medium | Medium |
| TC-REC-002 | Search for a recruitment candidate | High | High | Medium | Medium | Medium | Medium | Medium |
| TC-MYINFO-001 | View employee personal information | High | High | Medium | Medium | Medium | Medium | Medium |
| TC-MYINFO-002 | Update employee personal information | High | High | Medium | Medium | Medium | Medium | Medium |
| TC-DIR-001 | Search employee using Directory | High | High | Medium | Medium | Medium | Medium | Medium |
| TC-DIR-002 | View employee information from Directory | High | High | Medium | Medium | Medium | Medium | Medium |

## 4. High-Feasibility Scenarios

The following scenarios have a strong overall feasibility profile and are suitable for consideration in the initial automation scope:

- TC-LOGIN-001 to TC-LOGIN-007
- TC-DASH-001
- TC-ADMIN-001
- TC-ADMIN-002
- TC-ADMIN-003
- TC-PIM-001
- TC-PIM-002
- TC-PIM-004
- TC-PIM-005
- TC-PIM-006
- TC-PIM-007
- TC-PIM-008
- TC-LEAVE-001
- TC-LEAVE-002
- TC-LEAVE-003
- TC-LEAVE-004
- TC-LEAVE-005

These scenarios generally provide a combination of strong regression value, repeatability, predictable outcomes, and manageable automation effort.

## 5. Medium-Feasibility Scenarios

The following scenarios are technically feasible but require additional consideration before inclusion in the initial automation scope:

- TC-DASH-002
- TC-PIM-003
- TC-TIME-001
- TC-TIME-002
- TC-REC-001
- TC-REC-002
- TC-MYINFO-001
- TC-MYINFO-002
- TC-DIR-001
- TC-DIR-002

The primary considerations include lower initial regression value, test data requirements, workflow complexity, execution frequency, and maintenance effort.

## 6. Low-Feasibility Scenarios

No scenarios are classified as low feasibility at this stage.

The absence of low-feasibility scenarios does not mean that all scenarios will be automated. Final automation selection will also depend on prioritization, overall scope, project objectives, and available implementation effort.

## 7. Key Findings

The assessment indicates that the OrangeHRM application contains a strong set of technically feasible automation opportunities.

Core workflows involving authentication, employee management, and leave management provide the strongest combination of business value, repeatability, stability, and regression coverage.

Medium-feasibility scenarios may be considered as secondary automation coverage after the core regression suite is established.

## 8. Next Step

The feasibility assessment will be used as an input for final automation candidate prioritization.

The next stage will determine which feasible scenarios should receive the highest priority based on business risk, regression value, execution frequency, implementation effort, and overall automation ROI.

The prioritized scenarios will form the basis for defining the initial Playwright automation scope.