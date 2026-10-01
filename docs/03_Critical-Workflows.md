# OrangeHRM Critical Business 

**Author:** Jyothi Aradhya  
**Project:** OrangeHRM Playwright Automation Framework  
**Document:** Test Scenario Inventory

## 1. Purpose

This document identifies the key business workflows within the OrangeHRM application that are important for evaluating test automation coverage.

The workflows are identified based on business relevance, frequency of use, potential regression impact, and their importance to core HR operations.

Workflow identification does not represent a final automation decision. Individual test scenarios within these workflows will be evaluated separately for automation feasibility and priority.

## 2. Critical Business Workflows

| Workflow ID | Module | Business Workflow | Business Importance | Initial Priority |
|---|---|---|---|---|
| WF-01 | Login / Authentication | User Login and Authentication | Critical | High |
| WF-02 | Dashboard | Dashboard Access and Navigation | High | High |
| WF-03 | Admin | User and Role Management | High | Medium-High |
| WF-04 | PIM | Add Employee | Critical | High |
| WF-05 | PIM | Search and View Employee | High | High |
| WF-06 | PIM | Update Employee Information | High | High |
| WF-07 | Leave | Submit Leave Request | Critical | High |
| WF-08 | Leave | Leave Approval / Rejection | Critical | High |
| WF-09 | Time | Time / Attendance Workflow | High | Medium-High |
| WF-10 | Recruitment | Candidate Recruitment Workflow | High | Medium-High |
| WF-11 | My Info | Employee Self-Service / Personal Information | Medium | Medium |
| WF-12 | Directory | Employee Directory Search | Medium | Medium |

## 3. Workflow Prioritization

### High Priority

The following workflows are initially prioritized because they represent critical business operations, frequent user activities, or important regression scenarios:

- WF-01 – User Login and Authentication
- WF-02 – Dashboard Access and Navigation
- WF-04 – Add Employee
- WF-05 – Search and View Employee
- WF-06 – Update Employee Information
- WF-07 – Submit Leave Request
- WF-08 – Leave Approval / Rejection

### Medium-High Priority

These workflows are important but will require additional assessment before inclusion in the initial automation scope:

- WF-03 – User and Role Management
- WF-09 – Time / Attendance Workflow
- WF-10 – Candidate Recruitment Workflow

### Medium Priority

These workflows may be considered for automation after the core regression coverage is established:

- WF-11 – Employee Self-Service / Personal Information
- WF-12 – Employee Directory Search

## 4. Automation Consideration

The identified workflows provide the initial basis for test scenario analysis.

The final decision to automate a workflow or individual test case will depend on:

- Business criticality
- Execution frequency
- Repeatability
- Stability
- Regression value
- Technical feasibility
- Test data requirements
- Maintenance effort
- Automation ROI

The workflow list will therefore be refined during detailed test scenario and automation feasibility analysis.