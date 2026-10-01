# OrangeHRM Smoke Suite Definition

**Author:** Jyothi Aradhya  
**Project:** OrangeHRM Playwright Automation Framework  
**Document:** Smoke Suite Definition

## 1. Purpose

This document defines the initial automated smoke test suite for the OrangeHRM Playwright automation framework.

The smoke suite is intended to provide a fast and reliable validation of the application's critical functionality after a new build, deployment, environment change, or major application update.

The objective is to identify major application failures quickly before executing the broader regression suite.

## 2. Smoke Testing Objective

The primary objective of the smoke suite is to answer:

> Can the application support its most critical business workflows sufficiently to proceed with further testing?

Smoke testing focuses on a small set of high-value scenarios that validate:

- Application accessibility
- Authentication
- Successful application entry
- Core navigation
- Critical employee-management functionality
- Critical leave-management functionality

The smoke suite is not intended to provide complete functional or regression coverage.

## 3. Smoke Suite Selection Criteria

Test scenarios are considered for the smoke suite based on:

- Business criticality
- Application entry-point importance
- Core workflow dependency
- Regression impact
- Execution frequency
- Repeatability
- Stability
- Predictable expected results
- Fast execution
- Ability to identify major application failures early

Scenarios requiring extensive data preparation or complex workflows are generally not preferred for the initial smoke suite unless they provide sufficient business value.

## 4. Initial Smoke Test Scenarios

The initial OrangeHRM smoke suite will contain the following scenarios:

| Test Case ID | Test Scenario | Reason for Smoke Inclusion |
|---|---|---|

| TC-LOGIN-001 | Login with valid credentials | Validates the primary application entry point |

| TC-DASH-001 | Verify dashboard is displayed after successful login | Confirms successful application access after authentication |

| TC-PIM-001 | Add a new employee with valid details | Validates a critical employee-management workflow |

| TC-PIM-004 | Search for an existing employee | Validates core employee retrieval functionality |

| TC-PIM-007 | Update employee information | Validates a critical employee-management operation |

| TC-LEAVE-001 | Submit a leave request with valid details | Validates a critical leave-management workflow |

**Total initial smoke scenarios: 6**

## 5. Smoke Suite Rationale

### 5.1 Login

**TC-LOGIN-001 — Login with valid credentials**

Authentication is the primary entry point into the application.

If valid login functionality fails, most authenticated application workflows cannot be executed.

Therefore, this scenario is essential for smoke testing.

### 5.2 Dashboard

**TC-DASH-001 — Verify dashboard is displayed after successful login**

Successful authentication should result in access to the application's primary dashboard.

This validates that the application is not only accepting credentials but is also successfully loading the authenticated user experience.

### 5.3 Employee Creation

**TC-PIM-001 — Add a new employee with valid details**

Employee management represents a critical business capability.

Validating employee creation provides confidence that a major business workflow is operational.

### 5.4 Employee Search

**TC-PIM-004 — Search for an existing employee**

Employee retrieval is an important and frequently used operation.

Including this scenario provides additional validation of core PIM functionality without significantly increasing smoke execution time.

### 5.5 Employee Update

**TC-PIM-007 — Update employee information**

Updating employee information represents another critical employee-management operation.

Its inclusion helps validate that existing employee records can be modified successfully.

### 5.6 Leave Submission

**TC-LEAVE-001 — Submit a leave request with valid details**

Leave management is a critical HR business workflow.

Validating leave submission provides confidence that an important employee-facing process remains operational.

## 6. Smoke Suite Characteristics

The smoke suite should be:

- Small
- Fast
- Stable
- Repeatable
- Independent where practical
- Focused on critical functionality
- Suitable for frequent execution
- Capable of identifying major failures early

The suite should avoid unnecessary duplication of detailed functional validation.

## 7. Smoke Test Execution

The smoke suite may be executed:

- After a new deployment
- After a new application build
- After major environment changes
- Before broader regression execution
- As part of CI/CD validation
- During release validation

The exact execution trigger will be defined as part of the framework and CI/CD implementation.

## 8. Smoke Failure Handling

A failure in a critical smoke test should be investigated before proceeding with broader automated regression execution.

Examples include:

- Application cannot be accessed
- Valid login fails
- Dashboard does not load
- Critical employee workflow fails
- Critical leave workflow fails

Depending on the failure and project context, the broader regression suite may be:

- Blocked
- Investigated first
- Executed selectively for diagnostic purposes
- Continued when the failure is determined to be isolated

The final CI/CD failure-handling behavior will be defined during implementation.

## 9. Smoke Suite vs Regression Suite

Smoke testing and regression testing serve different purposes.

| Aspect | Smoke Suite | Regression Suite |
|---|---|---|

| Objective | Validate critical application health | Validate broader application behavior |

| Coverage | Small and focused | Broad |

| Execution Time | Short | Longer |

| Frequency | Frequently | As required |

| Test Selection | Critical workflows | Critical + extended scenarios |

| Failure Impact | May block further testing | Indicates functional regression |

| Primary Use | Build/deployment validation | Release/regression validation |

The smoke suite will therefore represent a subset of the broader automated regression suite.

## 10. Relationship to Initial Automation Scope

The six scenarios selected for the initial smoke suite are all part of the approved initial automation scope documented in the Final Automation Scope.

The smoke suite does not introduce new automation scope.

It represents a focused execution subset of the approved automation scenarios.

Additional smoke scenarios may be introduced if future business requirements or framework coverage justify their inclusion.

## 11. Future Smoke Suite Expansion

The smoke suite may be expanded when:

- Additional critical workflows are automated
- Business priorities change
- New critical functionality is introduced
- Regression risks change
- Application architecture changes
- CI/CD requirements evolve

Any significant change to the smoke suite should be documented and tracked through version control.

## 12. Success Criteria

The initial smoke suite will be considered effective when it:

- Executes reliably
- Completes within a practical time
- Detects major application failures early
- Provides clear pass/fail results
- Can be executed repeatedly
- Integrates effectively with the automation framework
- Can be used as an early validation stage in CI/CD

Detailed quantitative success metrics may be defined later during framework implementation.

## 13. Traceability

The smoke suite is derived from the following project documentation:

- Application Overview
- Module Inventory
- Critical Business Workflows
- Test Scenario Inventory
- Automation Candidate Assessment
- Manual-Only and Unsuitable Automation Scenarios
- Automation Feasibility Assessment
- Automation Prioritization
- Final Automation Scope
- Out-of-Scope Automation

This ensures that smoke test selection is based on documented business and automation analysis rather than implementation convenience alone.