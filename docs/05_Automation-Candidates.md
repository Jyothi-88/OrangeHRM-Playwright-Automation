# OrangeHRM Automation Candidate Assessment

**Author:** Jyothi Aradhya  
**Project:** OrangeHRM Playwright Automation Framework  
**Document:** Automation Candidate Assessment

## 1. Purpose

This document evaluates the test scenarios identified in the OrangeHRM Test Scenario Inventory to determine their suitability as potential automation candidates.

The assessment considers business value, execution frequency, repeatability, regression value, stability, technical feasibility, maintenance effort, and expected automation ROI.

Being identified as an automation candidate does not represent the final decision to include the scenario in the automation scope. Final selection will be determined through detailed feasibility assessment and prioritization.

## 2. Automation Candidate Assessment

| Test Case ID | Test Scenario | Automation Candidate | Initial Assessment |
|---|---|---|---|
| TC-LOGIN-001 | Login with valid credentials | Yes | Critical, repeatable, high regression value |
| TC-LOGIN-002 | Login with invalid username | Yes | Repeatable negative regression scenario |
| TC-LOGIN-003 | Login with invalid password | Yes | Repeatable negative regression scenario |
| TC-LOGIN-004 | Login with blank username | Yes | Stable validation scenario |
| TC-LOGIN-005 | Login with blank password | Yes | Stable validation scenario |
| TC-LOGIN-006 | Login with both fields blank | Yes | Repeatable validation scenario |
| TC-LOGIN-007 | Logout from the application | Yes | Common regression workflow |
| TC-DASH-001 | Verify dashboard is displayed after successful login | Yes | Critical post-login validation |
| TC-DASH-002 | Navigate between dashboard menu sections | Evaluate | Useful, but broad navigation may provide lower automation value |
| TC-ADMIN-001 | Create a new system user | Yes | Important administrative workflow |
| TC-ADMIN-002 | Search for an existing system user | Yes | Repeatable regression scenario |
| TC-ADMIN-003 | Validate required fields while creating a user | Yes | Stable negative validation |
| TC-PIM-001 | Add a new employee with valid details | Yes | Critical business workflow |
| TC-PIM-002 | Validate required fields while adding employee | Yes | Repeatable validation |
| TC-PIM-003 | Add employee with optional details | Evaluate | Useful but lower initial priority |
| TC-PIM-004 | Search for an existing employee | Yes | Frequent regression scenario |
| TC-PIM-005 | View employee details | Yes | Important functional validation |
| TC-PIM-006 | Search for a non-existing employee | Yes | Repeatable negative scenario |
| TC-PIM-007 | Update employee information | Yes | Important regression workflow |
| TC-PIM-008 | Validate updated employee information | Yes | Strong regression value |
| TC-LEAVE-001 | Submit a leave request with valid details | Yes | Critical business workflow |
| TC-LEAVE-002 | Validate leave request required fields | Yes | Stable negative validation |
| TC-LEAVE-003 | View submitted leave request | Yes | Repeatable workflow |
| TC-LEAVE-004 | Approve a pending leave request | Yes | Critical business workflow |
| TC-LEAVE-005 | Reject a pending leave request | Yes | Important regression scenario |
| TC-TIME-001 | Access Time/Attendance functionality | Evaluate | Page access alone provides moderate automation value |
| TC-TIME-002 | Submit a time-related entry | Evaluate | Requires assessment of data and workflow complexity |
| TC-REC-001 | Add a recruitment candidate | Evaluate | Valuable but not part of the initial core scope |
| TC-REC-002 | Search for a recruitment candidate | Evaluate | Useful but lower initial priority |
| TC-MYINFO-001 | View employee personal information | Evaluate | Moderate business and regression value |
| TC-MYINFO-002 | Update employee personal information | Evaluate | Valuable but not part of the initial core scope |
| TC-DIR-001 | Search employee using Directory | Evaluate | Useful but lower initial priority |
| TC-DIR-002 | View employee information from Directory | Evaluate | Moderate automation value |

## 3. Assessment Categories

### Automation Candidate — Yes

These scenarios have strong initial justification for automation based on factors such as:

- Business criticality
- Repeatability
- Regression value
- Predictable outcomes
- Stable functionality
- Potential execution frequency

### Automation Candidate — Evaluate

These scenarios may be suitable for automation but require additional assessment before final selection.

Factors requiring further evaluation include:

- Test data dependencies
- Workflow complexity
- Application stability
- Technical feasibility
- Maintenance effort
- Regression value
- Automation ROI

### Automation Candidate — No

No scenarios are classified as definite non-candidates at this stage.

Scenarios that may ultimately be excluded from automation will be identified during detailed manual-only analysis and feasibility assessment.

## 4. Decision Principles

The following principles will be used when determining whether a test scenario should be automated:

1. Automation should provide measurable testing value.
2. Repetitive and regression-focused scenarios should receive higher consideration.
3. Business-critical workflows should receive higher priority.
4. Stable and predictable scenarios are generally stronger automation candidates.
5. Technical feasibility and test data requirements must be considered.
6. Maintenance effort should be proportionate to the expected benefit.
7. Automation should not be pursued simply because a scenario can technically be automated.

## 5. Next Step

The identified automation candidates will undergo further assessment for:

- Manual-only suitability
- Technical feasibility
- Test data dependencies
- Stability
- Maintenance effort
- Automation ROI
- Final prioritization

The outcome of this assessment will be used to define the initial Playwright automation scope.