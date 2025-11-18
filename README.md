# urban-routes-web-testing
# 🧭 Urban Routes – Web Application Testing
Comprehensive manual and regression testing project for the Urban Routes web application.  
This project demonstrates professional QA documentation, structured test design, bug reporting, UI analysis, and SQL validation.

---

## 📌 Project Overview
Urban Routes is a web application for route planning and transportation services.  
The goal of this project was to evaluate its functionality, usability, and UI consistency through manual testing practices.

---

## 🧪 Scope of Testing
- Functional Testing  
- Regression Testing  
- UI/UX Testing  
- Cross-browser Testing  
- Requirements Analysis  
- SQL Data Validation  
- Bug Reporting using Jira  

---

## 🗂 Project Structure

---

## 📝 Test Case Example

```md
Test Case ID: TC-UR-045  
Title: Validate route creation with valid input  
Preconditions: User logged in  
Steps:
1. Open Urban Routes main page
2. Enter origin address
3. Enter destination address
4. Click "Calculate Route"

Expected Result:
Route is generated and displayed on the map.
Bug ID: BUG-UR-017  
Severity: High  
Title: Route calculation fails when destination field contains special characters  
Steps to Reproduce:
1. Open Urban Routes
2. Enter origin: "Park Avenue"
3. Enter destination: "@@@"

Expected:
Error validation message appears.

Actual:
Application freezes.

Evidence: /bug-reports/bug-report-017.pdf
SELECT user_id, route_id, created_at
FROM routes
WHERE user_id = 12345
ORDER BY created_at DESC;
