# OrangeHRM Module Inventory

**Author:** Jyothi Aradhya  
**Project:** OrangeHRM Playwright Automation Framework  
**Document:** Module Inventory

## 1. Purpose

This document identifies the major functional modules of the OrangeHRM application and establishes their initial priority for automation analysis.

The priorities listed here are preliminary. Final automation decisions will be made after detailed test scenario analysis and automation feasibility assessment.

## 2. Module Inventory

| ID | Module / Area | Business Relevance | Initial Automation Priority |
|---|---|---|---|
| MOD-01 | Login / Authentication | Critical | High |
| MOD-02 | Dashboard | High | High |
| MOD-03 | Admin | High | Medium-High |
| MOD-04 | PIM / Employee Management | Critical | High |
| MOD-05 | Leave | Critical | High |
| MOD-06 | Time | High | Medium-High |
| MOD-07 | Recruitment | High | Medium-High |
| MOD-08 | My Info | Medium | Medium |
| MOD-09 | Performance | Medium | Low / Later |
| MOD-10 | Directory | Medium | Medium |
| MOD-11 | Maintenance | Low / Administrative | Low / Later |
| MOD-12 | Buzz | Low | Low / Later |

## 3. Initial Priority Rationale

### High Priority

The following areas are initially considered high-priority candidates because they represent critical or frequently used workflows and are likely to provide significant regression value:

- Login / Authentication
- Dashboard
- PIM / Employee Management
- Leave

### Medium-High Priority

These areas may provide valuable automation coverage but will require further evaluation based on test stability, data dependencies, business value, and maintenance effort:

- Admin
- Time
- Recruitment

### Medium Priority

These areas may contain suitable automation candidates, but they are not the initial focus of the framework:

- My Info
- Directory

### Low / Later Priority

These areas will be considered after the core automation scope is established:

- Performance
- Maintenance
- Buzz

## 4. Automation Decision

Module priority does not automatically mean that all test cases within the module will be automated.

Individual test scenarios will be assessed based on:

- Business criticality
- Execution frequency
- Repeatability
- Stability
- Regression value
- Technical feasibility
- Test data requirements
- Maintenance effort
- Automation ROI

The final automation scope will be defined after test scenario analysis and feasibility assessment.