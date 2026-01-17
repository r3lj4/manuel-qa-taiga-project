# Test Scenarios – Taiga Manual QA Project

This document contains **high-level test scenarios** for manual testing of the Taiga web application.  
Each scenario describes a functionality or workflow to be tested.  
Detailed steps and expected results will be written later in the Test Cases.

---

## 1. User Authentication

### 1.1 User Registration
- Verify that a new user can successfully register
- Verify mandatory fields are validated
- Verify error messages are displayed for invalid input
- Verify successful registration redirects to dashboard

### 1.2 User Login
- Verify registered users can log in with correct credentials
- Verify error message appears for invalid credentials
- Verify password field is masked
- Verify “Remember Me” functionality (if available)

### 1.3 Logout
- Verify users can log out successfully
- Verify session ends after logout
- Verify redirect to login page

---

## 2. Project Management

### 2.1 Create Project
- Verify user can create a new project
- Verify project name validation (empty, duplicate, max length)
- Verify default project settings
- Verify project appears in user dashboard

### 2.2 Edit Project
- Verify user can edit project details
- Verify changes are saved correctly
- Verify invalid inputs are rejected

### 2.3 Delete Project
- Verify user can delete a project
- Verify confirmation prompt is displayed
- Verify project is removed from dashboard after deletion

---

## 3. Task & User Story Management

### 3.1 Create User Story
- Verify user can create a user story within a project
- Verify required fields (title, description, priority)
- Verify error messages for missing or invalid input

### 3.2 Edit User Story
- Verify user can edit existing user stories
- Verify updated information is saved and displayed

### 3.3 Delete User Story
- Verify user can delete a user story
- Verify confirmation prompt is displayed

### 3.4 Task Workflow
- Verify tasks can be created under user stories
- Verify tasks can move through statuses: New → In Progress → Done
- Verify completed tasks are visually distinguished
- Verify invalid status transitions are not allowed

---

## 4. UI & Usability

- Verify layout consistency across pages
- Verify navigation menus and buttons work as expected
- Verify error messages are clear and visible
- Verify form fields have proper labels and placeholders

---

## 5. Input Validation & Error Handling

- Verify mandatory fields cannot be left empty
- Verify max/min character limits are enforced
- Verify invalid input triggers error messages
- Verify system prevents actions on invalid state (e.g., deleting non-existing task)

---

## 6. Permissions & Access Control

- Verify regular users cannot access admin-only features
- Verify project members have correct access to projects/tasks
- Verify logged-out users cannot access protected pages
