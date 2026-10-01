# OrangeHRM Out-of-Scope Automation

**Author:** Jyothi Aradhya  
**Project:** OrangeHRM Playwright Automation Framework  
**Document:** Out-of-Scope Automation

## 1. Purpose

This document defines the functionality and test scenarios that are intentionally excluded from the initial OrangeHRM Playwright automation implementation.

The purpose is to establish a clear boundary for the initial automation scope and explain the reasoning behind scenarios that are deferred from implementation.

Being classified as out of scope does not mean that a scenario cannot be automated.

It means that the scenario is not part of the current implementation scope based on prioritization, business value, regression needs, feasibility, implementation effort, and expected automation ROI.

## 2. Relationship to Final Automation Scope

The initial automation scope was defined in the Final Automation Scope document.

The initial implementation focuses on:

- Login / Authentication
- Dashboard validation
- Selected Admin workflows
- Core PIM / Employee Management workflows
- Core Leave workflows

The scenarios documented here are intentionally deferred from the initial implementation.

They may be reconsidered during future framework expansion.

## 3. Out-of-Scope Scenarios

The following scenarios are outside the initial Playwright automation implementation scope:

| Test Case ID | Module | Test Scenario | Reason for Deferral |
|---|---|---|---|

| TC-DASH-002 | Dashboard | Navigate between dashboard menu sections | Lower initial automation value compared with core business workflows |

| TC-PIM-003 | PIM | Add employee with optional details | Lower initial priority compared with core employee workflows |

| TC-TIME-001 | Time | Access Time/Attendance functionality | Page access provides moderate regression value |

| TC-TIME-002 | Time | Submit a time-related entry | Requires additional consideration of workflow complexity and test data |

| TC-REC-001 | Recruitment | Add a recruitment candidate | Valuable but deferred to future automation expansion |

| TC-REC-002 | Recruitment | Search for a recruitment candidate | Lower initial priority compared with core HR workflows |

| TC-MYINFO-001 | My Info | View employee personal information | Moderate business and regression value |

| TC-MYINFO-002 | My Info | Update employee personal information | Valuable but deferred from the initial core scope |

| TC-DIR-001 | Directory | Search employee using Directory | Lower initial priority and moderate regression value |

| TC-DIR-002 | Directory | View employee information from Directory | Moderate automation value and deferred implementation priority |

## 4. Out-of-Scope Modules

The following modules are not part of the initial Playwright implementation scope:

| Module | Initial Status | Reason |
|---|---|---|

| Time | Out of Scope | Deferred until core regression coverage is established |

| Recruitment | Out of Scope | Deferred based on initial automation priority |

| My Info | Out of Scope | Moderate initial regression value |

| Directory | Out of Scope | Lower initial implementation priority |

| Performance | Out of Scope | Low initial automation priority |

| Maintenance | Out of Scope | Administrative functionality with lower initial regression priority |

| Buzz | Out of Scope | Low initial automation priority |

The Dashboard and PIM modules are partially in scope.

Only the scenarios specifically identified in the Final Automation Scope are included in the initial implementation.

## 5. Reasons for Exclusion

The primary reasons for excluding scenarios from the initial implementation include:

### 5.1 Lower Initial Regression Value

Some scenarios provide useful functional coverage but do not provide the same level of recurring regression value as the selected core workflows.

### 5.2 Lower Execution Priority

Some functionality is less frequently used or is not part of the highest-priority business workflows selected for the initial framework.

### 5.3 Workflow Complexity

Certain workflows require additional assessment of their implementation complexity, dependencies, or end-to-end data flow before automation.

### 5.4 Test Data Considerations

Some scenarios may require additional preparation, controlled data, or state management that is not necessary for the initial core suite.

### 5.5 Implementation Effort

The initial project has a defined implementation scope.

Adding lower-priority scenarios too early could increase implementation and maintenance effort before the core framework has been fully stabilized.

### 5.6 Automation ROI

Automation should provide measurable testing value.

Scenarios with lower expected ROI are deferred until the core regression suite provides sufficient coverage.

## 6. Manual Testing Responsibility

Out-of-scope automation does not mean that the functionality is excluded from testing.

These areas may continue to be covered through manual testing activities where appropriate.

Manual testing may include:

- Functional testing
- Exploratory testing
- Usability validation
- Ad-hoc investigation
- New functionality validation
- Regression testing where automation has not yet been implemented

The choice between manual and automated testing should continue to be based on testing value, risk, and business need.

## 7. Future Automation Consideration

Out-of-scope scenarios may be reconsidered when:

- Business priority increases
- Regression frequency increases
- The functionality becomes more stable
- Test data becomes easier to manage
- Automation feasibility improves
- Framework capabilities expand
- Maintenance effort becomes manageable
- Automation ROI becomes more favorable
- Additional regression coverage is required

Future inclusion will require reassessment rather than automatic promotion into the automation scope.

## 8. Scope Boundary

The initial Playwright implementation is intentionally limited to the scenarios defined in the Final Automation Scope document.

Functionality outside that scope will not be considered incomplete automation.

It represents a deliberate scope decision based on the project's current objectives and prioritization.

The purpose of the initial implementation is to establish a reliable, maintainable, and valuable automation foundation before expanding coverage.

## 9. Scope Governance

Any scenario proposed for inclusion after the initial implementation should be evaluated against the established automation decision criteria:

- Business criticality
- Regression value
- Execution frequency
- Repeatability
- Application stability
- Technical feasibility
- Test data requirements
- Maintenance effort
- Automation ROI

Approved scope changes should be reflected in the relevant documentation and version-control history.

## 10. Traceability

This out-of-scope assessment is based on the following project documentation:

- Application Overview
- Module Inventory
- Critical Business Workflows
- Test Scenario Inventory
- Automation Candidate Assessment
- Manual-Only and Unsuitable Automation Scenarios
- Automation Feasibility Assessment
- Automation Prioritization
- Final Automation Scope

This provides traceability between the initial analysis, prioritization decisions, and final automation boundaries.