# Test Plan – Taiga Manual QA Project

## 1. Introduction
This test plan describes the testing approach, scope, objectives, and resources for manual testing of the Taiga web application.  
The purpose of this document is to define how testing activities will be planned, executed, and documented.

---

## 2. Objectives
The main objectives of testing are:
- Verify that core functionalities work according to requirements
- Identify functional and UI defects
- Ensure critical workflows are stable
- Validate user-facing behavior from an end-user perspective

---

## 3. Application Under Test
- Application name: Taiga
- Type: Web-based project management tool
- URL: https://tree.taiga.io
- Authentication: Required

---

## 4. Scope of Testing

### In Scope
- User registration
- Login and logout
- Project creation
- User stories and task management
- Task status workflow
- Input validations
- UI behavior and error messages

### Out of Scope
- Performance testing
- Automation testing
- Security penetration testing
- Backend and database testing

---

## 5. Types of Testing
The following testing types will be performed:
- Functional testing
- Smoke testing
- Regression testing
- Exploratory testing
- Negative testing
- UI testing

---

## 6. Test Approach
Testing will be performed manually based on:
- User stories and application behavior
- Black-box testing techniques
- Predefined test scenarios and test cases
- Exploratory testing sessions

Black-box techniques used:
- Equivalence Partitioning
- Boundary Value Analysis
- Error Guessing

---

## 7. Test Environment
- Operating System: Linux
- Browsers: Chrome, Firefox
- Test Environment: Taiga public demo environment
- Network: Stable internet connection

---

## 8. Entry and Exit Criteria

### Entry Criteria
- Application is accessible
- Test environment is available
- Test scenarios and test cases are prepared

### Exit Criteria
- All planned test cases are executed
- Critical defects are reported
- Smoke and regression tests are completed

---

## 9. Defect Reporting
All identified defects will be documented with:
- Clear title
- Steps to reproduce
- Expected and actual results
- Severity and priority
- Supporting evidence (screenshots if applicable)

---

## 10. Risks and Mitigation

| Risk | Mitigation |
|----|----|
| Application changes | Focus on core stable functionality |
| Limited test data | Use multiple test accounts |
| Environment instability | Re-test critical flows |

---

## 11. Deliverables
- Test Plan
- Test Scenarios
- Test Cases
- Bug Reports
- Regression Checklist
- Exploratory Testing Notes

---

## 12. Approval
This test plan is created for learning and portfolio purposes and does not require formal approval.
