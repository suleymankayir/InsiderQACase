# Selenium Test Automation

This project contains automated tests for the Insider website using Selenium WebDriver, TestNG, and Java. The tests are designed to verify the functionality of the Careers and Home pages on the Insider website.

## Prerequisites

- Java JDK 8 or higher
- Maven
- IntelliJ IDEA or any other IDE
- WebDriverManager
- TestNG

## Project Structure

- `src/test/java/pages/`: Contains page object classes for the Insider website.
- `src/test/java/tests/`: Contains test classes for the Insider website.
- `src/test/java/utilities/`: Contains utility classes such as `Driver`, `ConfigReader`, and `ScreenShot`.

## Test Classes

### JobsPageTest

This class contains tests for the Careers page on the Insider website.

#### Test Method: `jobsTest`

1. Navigates to the Quality Assurance careers page.
2. Accepts cookies.
3. Clicks the "See all QA jobs" button.
4. Filters jobs by location ("Istanbul, Turkiye") and department ("Quality Assurance").
5. Verifies that the job list contains positions, departments, and locations matching the filters.
6. Clicks the "View Role" button and verifies that the user is redirected to the Lever application form page.
7. Takes a screenshot of the redirected page.
8. Closes the browser.

### HomePageTest

This class contains tests for the Home page on the Insider website.

#### Test Method: `homePageTests`

1. Navigates to the Insider home page.
2. Accepts cookies.
3. Verifies that the home page is displayed and takes a screenshot.
4. Selects the "Company" menu in the navigation bar and clicks the "Careers" submenu.
5. Verifies that the Careers page, its Locations, Teams, and Life at Insider blocks are displayed.
6. Closes the browser.

## Running the Tests

1. Clone the repository.
2. Open the project in IntelliJ IDEA or any other IDE.
3. Ensure that all dependencies are downloaded by running `mvn clean install`.
4. Run the test classes using TestNG.
