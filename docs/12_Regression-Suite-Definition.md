# OrangeHRM Regression Suite Definition

**Author:** Jyothi Aradhya

**Project:** OrangeHRM Playwright Automation Framework

**Document:** Regression Suite Definition

## 1. Purpose

This document defines the initial automated regression test suite for the OrangeHRM Playwright automation framework.

The regression suite is intended to validate that previously working functionality continues to operate correctly after application changes, enhancements, bug fixes, configuration changes, or new releases.

The regression suite provides broader functional coverage than the smoke suite and is designed to identify unintended impacts across critical and supporting business workflows.

## 2. Regression Testing Objective

The primary objective of the regression suite is to answer:

> Has the application's existing functionality remained stable after recent changes?

Regression testing focuses on automated scenarios that provide meaningful coverage of:

- Critical business workflows
- Frequently used functionality
- High-risk functionality
- Core employee-management operations
- Leave-management operations
- Authentication and access
- Important negative and validation scenarios
- Areas susceptible to regression

The regression suite is broader than the smoke suite but remains limited to scenarios that provide sufficient automation value.

## 3. Regression Suite Selection Criteria

Test scenarios are considered for the regression suite based on:

- Business criticality
- Regression risk
- Functional importance
- Frequency of use
- Repeatability
- Stability
- Automation feasibility
- Test data availability
- Predictable expected results
- Historical defect potential
- Maintenance effort
- Automation ROI

The regression suite should provide meaningful coverage without unnecessarily automating low-value or unstable scenarios.

## 4. Initial Regression Test Scenarios

The initial automated regression suite will be derived from the approved initial automation scope.

The following scenarios are included in the initial regression suite:

| Test Case ID | Test Scenario | Priority |
|---|---|---|
| TC-LOGIN-001 | Login with valid credentials | P0 |
| TC-LOGIN-002 | Login with invalid username | P1 |
| TC-LOGIN-003 | Login with invalid password | P1 |
| TC-LOGIN-004 | Login with blank username | P1 |
| TC-LOGIN-005 | Login with blank password | P1 |
| TC-LOGIN-006 | Login with both username and password blank | P1 |
| TC-LOGIN-007 | Logout from the application | P0 |
| TC-DASH-001 | Verify dashboard is displayed after successful login | P0 |
| TC-ADMIN-001 | Create a new system user | P1 |
| TC-ADMIN-002 | Search for an existing system user | P1 |
| TC-ADMIN-003 | Validate required fields while creating a system user | P1 |
| TC-PIM-001 | Add a new employee with valid details | P0 |
| TC-PIM-002 | Validate required fields while adding an employee | P1 |
| TC-PIM-004 | Search for an existing employee | P0 |
| TC-PIM-005 | View employee details | P0 |
| TC-PIM-006 | Search for a non-existing employee | P1 |
| TC-PIM-007 | Update employee information | P0 |
| TC-PIM-008 | Validate updated employee information | P0 |
| TC-LEAVE-001 | Submit a leave request with valid details | P0 |
| TC-LEAVE-002 | Validate required fields while submitting leave | P1 |
| TC-LEAVE-003 | View submitted leave | P0 |
| TC-LEAVE-004 | Approve a pending leave request | P0 |
| TC-LEAVE-005 | Reject a pending leave request | P0 |

**Total initial regression scenarios: 23**

## 5. Regression Suite Structure

The regression suite will be logically organized into priority-based and functional groups.

### 5.1 P0 Regression

P0 scenarios represent the highest-value regression coverage.

They validate critical business workflows and functionality where failure can significantly affect application usability or business operations.

Initial P0 regression scenarios include:

- Core authentication
- Dashboard access
- Employee creation
- Employee search
- Employee details
- Employee update
- Employee data validation
- Leave submission
- Leave viewing
- Leave approval
- Leave rejection

### 5.2 P1 Regression

P1 scenarios provide additional regression coverage for important validation, negative, and administrative workflows.

These include:

- Invalid login scenarios
- Blank login validation
- System user management
- Employee required-field validation
- Non-existing employee search
- Leave required-field validation

P1 scenarios complement the core P0 regression coverage.

## 6. Regression Suite vs Smoke Suite

The smoke suite and regression suite serve different purposes.

| Aspect | Smoke Suite | Regression Suite |
|---|---|---|
| Objective | Validate critical application health | Validate broader existing functionality |
| Coverage | Small and focused | Broader |
| Execution Time | Short | Longer |
| Test Selection | Most critical workflows | P0 + selected P1 workflows |
| Primary Trigger | Build/deployment validation | Changes, releases, regression cycles |
| Failure Meaning | May indicate application is not ready for further testing | Indicates potential functional regression |
| Scope | Subset of regression | Broader automated suite |

The smoke suite is therefore a subset of the initial regression suite.

## 7. Regression Execution Strategy

The regression suite may be executed:

- After significant application changes
- After feature enhancements
- After defect fixes
- Before a major release
- During release validation
- As part of scheduled CI/CD execution
- When changes affect critical business workflows
- When cross-module impact is suspected

The exact execution frequency will depend on project and CI/CD requirements.

## 8. Regression Failure Handling

When regression tests fail, the failure should be analyzed to determine whether it is caused by:

- A genuine application defect
- Test data issues
- Environment problems
- Locator or automation issues
- Timing or synchronization problems
- Configuration problems
- External dependency failures

Regression failures should not automatically be classified as application defects.

Failures should be investigated using available automation diagnostics such as:

- Test execution logs
- Screenshots
- Traces
- Videos where configured
- HTML reports
- Error messages
- Environment information

Confirmed application defects should be documented through the appropriate defect-management process.

## 9. Regression Suite Maintenance

The regression suite should be reviewed periodically to ensure continued relevance and reliability.

Maintenance activities may include:

- Updating tests for application changes
- Removing obsolete scenarios
- Adding newly critical scenarios
- Improving unstable tests
- Reviewing duplicate coverage
- Updating test data
- Reassessing automation ROI
- Reviewing execution time
- Reviewing failure trends
- Reprioritizing scenarios when business risk changes

Regression suite maintenance is considered part of automation framework ownership.

## 10. Regression Suite and Test Data

Regression execution depends on reliable and repeatable test data.

Test data should be:

- Clearly identified
- Reusable where appropriate
- Maintainable
- Independent where practical
- Suitable for repeated execution
- Protected from unintended test interference

Where workflows modify application data, the framework should consider appropriate test-data management and cleanup strategies.

The detailed test-data architecture will be defined during framework implementation.

## 11. Relationship to Initial Automation Scope

All 23 scenarios in the initial regression suite belong to the approved initial automation scope.

The regression suite does not expand the approved automation scope.

It defines how the approved automated scenarios will be grouped and executed for regression validation.

The 10 P2 scenarios documented as out-of-scope remain excluded from the initial regression suite.

## 12. Future Regression Expansion

The regression suite may be expanded when:

- Additional high-value workflows are automated
- P2 scenarios are brought into scope
- New critical functionality is introduced
- Business risk changes
- New regression risks are identified
- Defect trends indicate additional coverage is required
- Application architecture changes
- CI/CD execution requirements evolve

Any significant change to the regression suite should be documented and maintained through version control.

## 13. Success Criteria

The initial regression suite will be considered effective when it:

- Provides meaningful coverage of approved automation scope
- Detects important regressions
- Executes reliably
- Produces clear results
- Can be executed repeatedly
- Maintains acceptable execution time
- Minimizes false failures
- Supports release confidence
- Integrates effectively with CI/CD

Detailed quantitative metrics may be defined later during framework implementation.

## 14. Traceability

The regression suite is derived from the following project documentation:

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
- Smoke Suite Definition

This ensures that regression coverage is based on documented business risk, automation feasibility, and prioritization rather than implementation convenience alone.