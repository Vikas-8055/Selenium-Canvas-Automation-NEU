# Selenium Canvas Automation NEU

This project is developed as part of the INFO6255 – Software Quality Control and Management course at Northeastern University (Spring 2025). It automates various student-facing workflows using Selenium WebDriver, TestNG, and a data-driven testing approach.

---

## 📘 Description

The framework automates key student services across NEU platforms using:
- Java with Maven
- Selenium WebDriver
- TestNG as the test runner
- Excel-driven test inputs
- Automated screenshots
- HTML-style reporting

---

## ✅ Test Scenarios

1. **Scenario 1** – Download latest transcript from Student Hub  
2. **Scenario 2** – Add Canvas Calendar To-Do tasks  
3. **Scenario 3** – Reserve study room at Snell Library  
4. **Scenario 4** – Download dataset from NU Library DRS  
5. **Scenario 5** – Update and verify Academic Calendar  

---

## 📂 Project Structure

Selenium-Canvas-Automation-NEU-main/ ├── pom.xml # Maven config and dependencies ├── /src/ │ ├── /main/java/com/sqcm/group4/Selenium/ │ │ ├── pages/ # Page Object classes (LoginPage, TranscriptPage, etc.) │ │ └── utils/ # Excel reader, ReportManager, ScreenshotManager │ └── /test/ │ ├── /java/com/sqcm/group4/Selenium/ │ │ └── *.java # Scenario test classes (one per scenario) │ └── /resources/ │ ├── testng.xml # TestNG suite configuration │ └── test_data.xlsx # External test data file ├── /screenshots/ │ ├── /Scenario1/ │ ├── /Scenario2/ │ ├── /Scenario3/ │ ├── /Scenario4/ │ └── /Scenario5/ ├── /downloads/ # PDF/ZIP downloads saved during tests ├── /allure-results/ # JSON logs for Allure report

## 📦 Example for Scenario 4
Selenium-Canvas-Automation-NEU-main/ ├── pom.xml ├── /src/test/java/scenarios/ │ └── Scenario4DownloadDataset.java ├── /screenshots/Scenario4/ ├── /downloads/


**📝 Notes**

Fully data-driven: no hardcoded values

Screenshots captured before and after each action

Assertions and verifications implemented in all test cases

Designed using the Page Object Model for modularity
---

## 🚀 How to Run

### Option 1: From IDE (Recommended)

#### ▶ To run all scenarios continuously:
1. **Right-click the entire project folder**: `Selenium-Canvas-Automation-NEU-main/`
2. Choose **Run As → TestNG Suite**  
   This will trigger all test classes as per the `testng.xml` suite file.

#### ▶ To run a single test:
1. Right-click any test class (e.g., `Scenario4DownloadDataset.java`)
2. Choose **Run As → TestNG Test**

---

### Option 2: From Terminal

Make sure Maven is installed and configured:

```bash
cd Selenium-Canvas-Automation-NEU-main
mvn clean test

