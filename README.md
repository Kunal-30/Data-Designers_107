**README for Automation Projects**

*Introduction*

This repository contains two automation projects:

1. **Performance Testing using JMeter**: Automates performance testing for the DummyJSON API, validating various HTTP requests for "Comments" and "Recipes" endpoints.
2. **UI Automation for Bus Ticket Booking**: Automates the complete flow of booking bus tickets on the SMBus website using Selenium with the Page Object Model (POM) framework.

*Project 1: Performance Testing using JMeter*

Objective

The objective is to perform performance testing by automating various HTTP requests (GET, POST, PUT, DELETE) on the DummyJSON API endpoints for Comments and Recipes.

Setup and Requirements

1. Install Apache JMeter.
2. Ensure Firefox is installed for recording test steps.
3. Familiarize yourself with JMeter components like Samplers, Listeners, and Debug Samplers.

Tasks Implemented

- Validated Recipes requests:
  - Get all recipes, Get a single recipe, Search recipes, Limit & Skip recipes, Sort recipes, Get recipes by tag, and Get recipes by meal.
- Validated Comments requests:
  - Get all comments, Get a single comment, Limit & Skip comments, Get comment by post ID, Add, Update, and Delete a comment.

Framework Details

- Used Regular Expressions for dynamic extraction.
- Configured multiple threads, ramp-up time, and infinite loops for performance analysis.
- Included Aggregate Report and other listeners for result analysis.
- Comments added to explain each section of the JMeter configuration.

*Project 2: UI Automation for Bus Ticket Booking* 

Objective

The objective is to automate the process of booking bus tickets on the SMBus website, starting from selecting cities and date to booking a seat.

Setup and Requirements

1. Install Java, Maven, and TestNG.
2. Clone this repository and open it in your preferred IDE (e.g., IntelliJ, Eclipse).
3. Use the Maven `pom.xml` file to manage dependencies.

Framework Details

- Implemented Page Object Model (POM) to manage page elements.
- Test scripts written using TestNG annotations.
- Configured Maven for dependency management and project execution.
- Read test data (e.g., URLs) from a property file.
- Used Explicit and Implicit Waits for synchronization.
- Assertions used for validation.
- Captured screenshots for specific steps.
- Generated Extent Reports for test execution summary.

Tasks Implemented

1. Selected cities (From and To) and date from the calendar.
2. Searched for buses and asserted bus details from UI.
3. Captured screenshots of Rest Stops, Amenities, Cancellation Terms, Boarding and Dropping points.
4. Displayed seat availability and booked a seat.
5. Automated the entire flow using POM, TestNG, and Maven.

Execution

1. Clone the repository.
2. Execute tests using the Maven command: `mvn test`.
3. View Extent Reports in the `Reports` folder.

Submission
Push the project to a new GitHub repository and share the repository link.
