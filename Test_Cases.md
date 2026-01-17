# Test Cases – Taiga Manual QA Project

This document contains **detailed manual test cases** for the Taiga web application.  
Each test case is linked to a high-level scenario from `Test_Scenarios.md`.

---

## 1. User Authentication

### TC-01: User Registration – Valid Input
- **Preconditions:** User is on the Taiga registration page  
- **Steps:**  
  1. Enter valid username, email, and password  
  2. Click "Register" button  
- **Expected Result:**  
  - User is registered successfully  
  - Redirected to dashboard  
  - Confirmation message is displayed  

### TC-02: User Registration – Invalid Input
- **Preconditions:** User is on the registration page  
- **Steps:**  
  1. Leave mandatory fields empty or enter invalid email  
  2. Click "Register" button  
- **Expected Result:**  
  - Appropriate error messages appear for each invalid input  
  - User is not registered  

### TC-03: Login – Valid Credentials
- **Preconditions:** User is registered  
- **Steps:**  
  1. Enter registered email and password  
  2. Click "Login" button  
- **Expected Result:**  
  - User is logged in successfully  
  - Dashboard page is displayed  

### TC-04: Login – Invalid Credentials
- **Preconditions:** User is on login page  
- **Steps:**  
  1. Enter incorrect email or password  
  2. Click "Login" button  
- **Expected Result:**  
  - Error message displayed: "Invalid email or password"  
  - User remains on login page  

### TC-05: Logout
- **Preconditions:** User is logged in  
- **Steps:**  
  1. Click "Logout" button  
- **Expected Result:**  
  - User is logged out successfully  
  - Redirected to login page  

---

## 2. Project Management

### TC-06: Create Project – Valid Input
- **Preconditions:** User is logged in  
- **Steps:**  
  1. Navigate to "Create Project" page  
  2. Enter valid project name and description  
  3. Click "Create" button  
- **Expected Result:**  
  - Project is created  
  - Appears in dashboard  
  - Confirmation message displayed  

### TC-07: Create Project – Invalid Input
- **Preconditions:** User is on Create Project page  
- **Steps:**  
  1. Leave project name empty or use duplicate name  
  2. Click "Create" button  
- **Expected Result:**  
  - Error message displayed  
  - Project is not created  

### TC-08: Edit Project
- **Preconditions:** User has at least one project  
- **Steps:**  
  1. Open project  
  2. Edit project name or description  
  3. Click "Save" button  
- **Expected Result:**  
  - Changes are saved and visible  
  - No errors occur  

### TC-09: Delete Project
- **Preconditions:** User has at least one project  
- **Steps:**  
  1. Click "Delete Project"  
  2. Confirm deletion  
- **Expected Result:**  
  - Project is removed from dashboard  
  - Confirmation message displayed  

---

## 3. User Stories & Task Management

### TC-10: Create User Story
- **Preconditions:** User is in a project  
- **Steps:**  
  1. Navigate to "User Stories" section  
  2. Click "Create Story"  
  3. Enter valid title and description  
  4. Click "Save"  
- **Expected Result:**  
  - Story is created successfully  
  - Appears in project backlog  

### TC-11: Edit User Story
- **Preconditions:** At least one user story exists  
- **Steps:**  
  1. Open a story  
  2. Edit title or description  
  3. Click "Save"  
- **Expected Result:**  
  - Story updates are saved and visible  

### TC-12: Delete User Story
- **Preconditions:** At least one user story exists  
- **Steps:**  
  1. Click "Delete Story"  
  2. Confirm deletion  
- **Expected Result:**  
  - Story is removed from backlog  
  - Confirmation message displayed  

### TC-13: Task Workflow
- **Preconditions:** At least one user story exists  
- **Steps:**  
  1. Create a task under a user story  
  2. Move task through statuses: New → In Progress → Done  
- **Expected Result:**  
  - Task changes status correctly  
  - Done tasks are visually distinct  

---

## 4. UI & Input Validation

### TC-14: UI Layout
- **Preconditions:** User is logged in  
- **Steps:**  
  1. Navigate through main pages (Dashboard, Project, Backlog)  
- **Expected Result:**  
  - Layout is consistent  
  - Buttons, menus, and links work  
  - No overlapping elements  

### TC-15: Input Validation
- **Preconditions:** User is creating project/story/task  
- **Steps:**  
  1. Leave mandatory fields empty  
  2. Enter too long text or invalid characters  
- **Expected Result:**  
  - Error messages are displayed  
  - System prevents invalid submission  
