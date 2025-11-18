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

---

# 🛒 **2. URBAN GROCERS — API Automation Project**  
📁 **Repo name:** `urban-grocers-api-testing`

---

## 🟩 **README PARA PEGAR**

```md
# 🛒 Urban Grocers – API Testing & Automation
API testing and automation project for the Urban Grocers REST API.  
Includes manual API validation, automated test scripts (Pytest), Postman collections, and documentation.

---

## 🚀 Scope
- API Functional Testing  
- Automation with Pytest (Python)  
- JSON response validation  
- Negative testing  
- Authentication testing  
- Bug reporting  
- Git version control  

---

## 📂 Project Structure


---

## 🧪 Pytest Automation Example

```python
import requests

BASE_URL = "https://urban-grocers.com/api"

def test_create_order_success():
    payload = {
        "user_id": 12,
        "items": ["milk", "bread"],
        "payment_method": "card"
    }
    
    response = requests.post(f"{BASE_URL}/orders", json=payload)
    
    assert response.status_code == 201
    json_resp = response.json()
    assert "order_id" in json_resp
GET /orders/123

Expected Response:
{
  "order_id": 123,
  "status": "delivered",
  "items": ["milk", "bread"]
}

---

# 🍔 **3. URBAN LUNCH — Mobile Testing**  
📁 **Repo name:** `urban-lunch-mobile-testing`

---

## 🟩 **README PARA PEGAR**

```md
# 🍔 Urban Lunch – Mobile Testing Project
Mobile QA project testing the Urban Lunch Android application using Android Studio.

---

## 🎯 Scope
- Functional Testing  
- Exploratory Testing  
- Performance & UI Validation  
- End-to-end user flows  
- Defect documentation  

---

## 📂 Structure


---

## 📝 Example Test Flow

```md
Flow: Order Creation

1. Open the app  
2. Select a restaurant  
3. Add item to cart  
4. Complete payment  

Expected:  
Order confirmation screen appears.
Bug: App crashes when selecting "Payment with Card"  
Device: API Level 33 - Pixel 6  
Severity: Critical  

---

# 🛵 **4. SCOOTER — Full End-to-End Testing**  
📁 **Repo name:** `scooter-e2e-testing`

---

## 🟩 **README PARA PEGAR**

```md
# 🛵 Scooter – Full End-to-End QA Project

Comprehensive QA project covering Web Testing, Mobile Testing, API Testing, SQL Validation, and Automation for the Scooter application.

---

## 📌 Scope
- Web Testing  
- API Testing (Postman)  
- SQL Validation  
- Mobile Testing  
- Automation (Pytest + Selenium)  
- Exploratory Testing  
- Documentation & Reporting  

---

## 📂 Project Structure


---

## 🧪 Selenium Example

```python
from selenium import webdriver

def test_login_success():
    driver = webdriver.Chrome()
    driver.get("https://scooter-app.com/login")

    driver.find_element("id","email").send_keys("test@test.com")
    driver.find_element("id","password").send_keys("123456")

    driver.find_element("id","login-btn").click()

    assert "dashboard" in driver.current_url
    driver.quit()

---

# 🎉 ¿QUIERES QUE TAMBIÉN TE ENTREGO…?

✅ Los **archivos reales** (`test-cases.xlsx`, `sql`, `Postman`, etc.)  
✅ Las **imágenes de evidencia falsas pero profesionales**  
✅ Un **index.html** para tu portafolio  
✅ Los **repos listos en formato ZIP**  

Solo dime:  
**¿Quieres que genere los archivos (Excel, SQL, JSON, Python) para descargarlos y subirlos?**

