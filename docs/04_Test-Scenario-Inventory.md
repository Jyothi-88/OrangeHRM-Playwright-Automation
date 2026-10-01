# OrangeHRM Test Scenario Inventory

**Author:** Jyothi Aradhya  
**Project:** OrangeHRM Playwright Automation Framework  
**Document:** Test Scenario Inventory

## 1. Purpose

This document provides an inventory of test scenarios derived from the critical business workflows identified for the OrangeHRM application.

The inventory serves as the foundation for evaluating test scenarios for automation feasibility, prioritization, and inclusion in the Playwright automation scope.

The scenarios cover positive, negative, and functional testing across the identified business workflows.

## 2. Test Scenario Inventory

| Test Case ID | Workflow ID | Test Scenario | Test Type | Priority |
|---|---|---|---|---|
| TC-LOGIN-001 | WF-01 | Login with valid credentials | Positive | Critical |
| TC-LOGIN-002 | WF-01 | Login with invalid username | Negative | High |
| TC-LOGIN-003 | WF-01 | Login with invalid password | Negative | High |
| TC-LOGIN-004 | WF-01 | Login with blank username | Negative | High |
| TC-LOGIN-005 | WF-01 | Login with blank password | Negative | High |
| TC-LOGIN-006 | WF-01 | Login with both fields blank | Negative | Medium |
| TC-LOGIN-007 | WF-01 | Logout from the application | Positive | High |
| TC-DASH-001 | WF-02 | Verify dashboard is displayed after successful login | Positive | High |
| TC-DASH-002 | WF-02 | Navigate between dashboard menu sections | Functional | Medium |
| TC-ADMIN-001 | WF-03 | Create a new system user | Positive | High |
| TC-ADMIN-002 | WF-03 | Search for an existing system user | Functional | High |
| TC-ADMIN-003 | WF-03 | Validate required fields while creating a user | Negative | Medium |
| TC-PIM-001 | WF-04 | Add a new employee with valid details | Positive | Critical |
| TC-PIM-002 | WF-04 | Validate required fields while adding employee | Negative | High |
| TC-PIM-003 | WF-04 | Add employee with optional details | Positive | Medium |
| TC-PIM-004 | WF-05 | Search for an existing employee | Functional | High |
| TC-PIM-005 | WF-05 | View employee details | Functional | High |
| TC-PIM-006 | WF-05 | Search for a non-existing employee | Negative | Medium |
| TC-PIM-007 | WF-06 | Update employee information | Positive | High |
| TC-PIM-008 | WF-06 | Validate updated employee information | Functional | High |
| TC-LEAVE-001 | WF-07 | Submit a leave request with valid details | Positive | Critical |
| TC-LEAVE-002 | WF-07 | Validate leave request required fields | Negative | High |
| TC-LEAVE-003 | WF-07 | View submitted leave request | Functional | High |
| TC-LEAVE-004 | WF-08 | Approve a pending leave request | Positive | Critical |
| TC-LEAVE-005 | WF-08 | Reject a pending leave request | Positive | High |
| TC-TIME-001 | WF-09 | Access Time/Attendance functionality | Functional | Medium-High |
| TC-TIME-002 | WF-09 | Submit a time-related entry | Positive | Medium |
| TC-REC-001 | WF-10 | Add a recruitment candidate | Positive | Medium-High |
| TC-REC-002 | WF-10 | Search for a recruitment candidate | Functional | Medium |
| TC-MYINFO-001 | WF-11 | View employee personal information | Functional | Medium |
| TC-MYINFO-002 | WF-11 | Update employee personal information | Positive | Medium |
| TC-DIR-001 | WF-12 | Search employee using Directory | Functional | Medium |
| TC-DIR-002 | WF-12 | View employee information from Directory | Functional | Medium |

## 3. Test Scenario Classification

The identified scenarios are categorized into the following test types:

- **Positive Testing** – Valid inputs and expected successful workflows.
- **Negative Testing** – Invalid inputs, missing information, and error-handling scenarios.
- **Functional Testing** – Verification of specific application functionality and expected behavior.

## 4. Prioritization

Test scenario priority is based on the following factors:

- Business criticality
- Potential regression impact
- Frequency of execution
- Importance of the associated workflow
- User impact

The priority assigned at this stage is an initial assessment and may be revised during automation feasibility and candidate prioritization.

## 5. Automation Assessment

The scenarios listed in this document have not yet been designated as automation candidates.

Each scenario will be evaluated separately based on:

- Business criticality
- Execution frequency
- Repeatability
- Stability
- Regression value
- Technical feasibility
- Test data requirements
- Maintenance effort
- Automation ROI

The outcome of this assessment will determine which scenarios become automation candidates and which scenarios are excluded from the initial Playwright automation scope.
