# OrangeHRM Manual-Only and Unsuitable Automation Scenarios

**Author:** Jyothi Aradhya  
**Project:** OrangeHRM Playwright Automation Framework  
**Document:** Manual-Only and Unsuitable Automation Scenarios

## 1. Purpose

This document defines the types of testing activities and scenarios that may be better suited to manual testing rather than UI automation.

The purpose is to ensure that automation is applied selectively where it provides meaningful value and that manual testing continues to be used where human judgment, exploration, or adaptability provides greater benefit.

## 2. Scenarios Generally Better Suited to Manual Testing

The following types of scenarios may be better suited to manual testing:

| Scenario Type | Reason for Manual Preference |
|---|---|
| Exploratory Testing | Requires human investigation, observation, and adaptive decision-making |
| Usability Evaluation | Requires human judgment of user experience and ease of use |
| Subjective Visual Assessment | Human perception may be required to evaluate visual quality and presentation |
| Ad-hoc Investigation | Short-lived or investigative activities may not provide sufficient automation ROI |
| One-Time Validation | Low execution frequency may not justify automation effort and maintenance |
| Frequently Changing Functionality | Automation may require excessive maintenance while requirements or UI behavior are unstable |
| Unclear or Evolving Requirements | Expected results may change frequently, reducing the value of automated scripts |

## 3. Assessment of Current Test Scenario Inventory

The current OrangeHRM test scenario inventory does not contain any scenarios that are classified as permanently manual-only at this stage.

The majority of the identified scenarios have:

- Objective expected results
- Repeatable execution steps
- Potential regression value
- Potential for reliable automated validation

Therefore, they remain eligible for further automation assessment.

## 4. Scenarios Requiring Further Evaluation

Some scenarios currently classified as "Evaluate" in the Automation Candidate Assessment may ultimately remain outside the initial automation scope.

The final decision will depend on:

- Technical feasibility
- Test data dependencies
- Application stability
- Execution frequency
- Regression value
- Maintenance effort
- Automation ROI
- Overall business value

A scenario being excluded from the initial automation scope does not necessarily mean it must always be tested manually.

It may be reconsidered as application stability, requirements, automation coverage, or business priorities change.

## 5. Manual Testing and Automation Strategy

Manual testing and automation are complementary activities.

Automation will be used primarily for repeatable, stable, business-critical, and regression-focused scenarios.

Manual testing will continue to provide value for:

- Exploratory testing
- Usability evaluation
- Subjective validation
- Ad-hoc investigation
- Scenarios where automation ROI is low
- New or rapidly changing functionality

The objective is to establish an appropriate balance between automated and manual testing rather than attempting to automate all testing activities.

## 6. Decision Principle

The decision to keep a scenario manual should be based on testing value and risk rather than the technical ability to automate it.

Automation should be avoided when the expected maintenance effort significantly exceeds the testing benefit.