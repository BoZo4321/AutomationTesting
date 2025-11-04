# Vikta UI Test Automation Framework

This repository contains my educational **UI test automation framework** for the **Vikta web application**, originally developed as part of an internship practice at Grid Dynamics.

The framework was created for learning and demonstrating **automated GUI testing** using **Java, Selenium, Selenide, and TestNG**.  
It does **not include** the original Vikta web application, its **Docker environment**, or **MySQL database**, because those are internal components of the company setup.  
This repository focuses solely on the **automation framework** layer — the structure, code, and logic for test execution and reporting.

---

##  Project Overview

This project demonstrates how to design and implement a structured, maintainable **test automation framework** in Java following modern best practices.  
The framework follows the **Page Object Model (POM)** design pattern, which separates UI locators and actions from test logic, improving code readability and scalability.

Even without the actual Vikta application, the project can serve as a reference for building a full-featured automation suite for any web application with login, registration, and home functionalities.

---

##  Technologies Used

| Purpose | Tool / Library | Description |
|----------|----------------|--------------|
| **Programming Language** | Java 8+ | Core language for test logic and framework structure |
| **Test Framework** | TestNG | Handles test execution, annotations, and grouping |
| **UI Automation** | Selenium & Selenide | Provides WebDriver control and fluent APIs for UI interaction |
| **Reporting** | Allure Report | Generates detailed and interactive test execution reports |
| **Logging** | Log4j | Manages application and test run logs |
| **Build Tool** | Maven | Dependency management and project build automation |
| **Lombok** | Lombok Plugin | Reduces boilerplate code such as getters/setters |

---

**Key folders:**
- `pageObjects/` – defines each web page as an object with locators and methods.  
- `stepsDefinitions/` – contains logic for user actions and flow steps.  
- `tests/` – includes actual TestNG tests calling step definitions.  
- `resources/` – configuration files for Allure, app setup, and logging.

---

##  Using IntelliJ IDEA

1. Open the project in IntelliJ IDEA.  
2. Create a **TestNG Run/Debug Configuration**.  
3. Run or debug the selected test.

---

##  Generating Allure Report

After test execution, you can generate an interactive Allure report with:

```bash
allure serve
```
This command will start a local Allure server and open a visual test results dashboard in your browser.

##  About Missing Components

The original **Vikta application**, its **Docker container**, and **MySQL database** are **not included** in this repository because they are internal to the company infrastructure and require authentication credentials.

However, the entire **test automation layer** is preserved here, showing:

- Page Object structure  
- TestNG test execution  
- Allure report integration  
- Configuration and logging setup  

This makes it a fully functional example of a **UI test automation framework** that can be easily adapted to other applications.

---

##  Learning Focus

This project demonstrates:

- How to design a modular automation framework in **Java**  
- How to use the **Page Object Model (POM)** pattern  
- Step-based separation between **UI actions** and **test logic**  
- Integration with **Allure reporting** and **Log4j logging**  
- **Maven** project structure and lifecycle configuration  
- Best practices for maintainable test code  

---

##  Author

**Božidar Radosavljević**  
QA Engineer & Java Developer  

Educational project inspired by internship work at Grid Dynamics — focused on developing a strong understanding of **Java-based UI automation frameworks**.

##  Useful References

- [Selenium Documentation](https://www.selenium.dev/documentation/)  
- [Selenide Documentation](https://selenide.org/documentation.html)  
- [TestNG Official Docs](https://testng.org/doc/)  
- [Baeldung – TestNG Overview](https://www.baeldung.com/testng)  
- [Baeldung – Java Selenium Examples](https://www.baeldung.com/selenium)  
- [Project Lombok](https://projectlombok.org/)  
- [Page Object Model Concepts](https://www.toolsqa.com/selenium-webdriver/page-object-model/)
