# STQA

ANSWER 1: TEST PLAN
Sr. No.	Test Plan Point	Answer
1	Test Plan Identifier	Test Plan ID: MILKAPP_TP_V1.0
Prepared by: QA Team
Date: 12-Nov-2025
2	References	• Software Requirements Specification (SRS) for Online Milk Ordering App
* Design Document
* IEEE 829 Standard for Software Test Documentation
* Project Plan Document
3	Introduction	The Online Milk Ordering Mobile Application allows users to register, log in, view milk quantity, price, available discounts, and estimated delivery time. The purpose of this test plan is to define the scope, objectives, approach, environment, schedule, and responsibilities for testing this application to ensure its quality and reliability.
4	Features to be Tested	• User Registration (valid/invalid input)
* Login authentication
* Checking milk quantity availability
* Display of price and discounts
* Delivery time estimation
* Order placement and confirmation
* Logout functionality
5	Approach	• Testing Type: Manual Functional Testing
* Techniques Used: Boundary Value Analysis, Equivalence Partitioning, Positive and Negative Testing
* Levels of Testing: Unit Testing, Integration Testing, System Testing, User Acceptance Testing
* Test Data: Valid and invalid input data for all modules
* Defect Tracking using standard bug reporting tool
6	Environmental Needs	• Hardware: Android/iOS smartphones
* Software: Android Studio Emulator, iOS Simulator
* Database: MySQL (Cloud)
* Network: Wi-Fi and 4G connections
* Test Data: Dummy user profiles, sample product data
7	Staffing & Training Needs	• Team Members: Test Manager, QA Lead, Test Engineers
* Training Needs: Application domain understanding, test tool usage, mobile testing techniques
* Experience Required: Familiarity with functional and UI testing of mobile apps
8	Responsibilities	
9	Schedule	
10	Approval	Test Plan Prepared By: QA Team
Reviewed By: Test Manager
Approved By: Project Manager / Client
Date of Approval: _______

| *Sr. No.* | *Test Case ID* | *Test Scenario / Step*                          | *Test Data*                                                                     | *Expected Result*                                                 | *Actual Result* | *Pass / Fail* |
| ----------- | ---------------- | ------------------------------------------------- | --------------------------------------------------------------------------------- | ------------------------------------------------------------------- | ----------------- | --------------- |
| 1           | TC01             | Verify registration with valid details            | Name: Rahul, Email: [rahul@gmail.com](mailto:rahul@gmail.com), Password: Test@123 | User should be registered successfully and redirected to login page | As per test       | Pass/Fail       |
| 2           | TC02             | Verify registration with already used email       | Email: [rahul@gmail.com](mailto:rahul@gmail.com)                                  | System should display “Email already exists”                        | As per test       | Pass/Fail       |
| 3           | TC03             | Verify registration with missing mandatory fields | Email: (blank), Password: 123                                                     | System should display “Email is required” message                   | As per test       | Pass/Fail       |
| 4           | TC04             | Verify login with valid credentials               | Email: [rahul@gmail.com](mailto:rahul@gmail.com), Password: Test@123              | User should be redirected to Home Screen                            | As per test       | Pass/Fail       |
| 5           | TC05             | Verify login with invalid credentials             | Email: [rahul@gmail.com](mailto:rahul@gmail.com), Password: wrong123              | System should show “Invalid credentials”                            | As per test       | Pass/Fail       |
| 6           | TC06             | Verify milk quantity selection updates correctly  | Quantity selected: 2 litres                                                       | Displayed quantity = 2 litres                                       | As per test       | Pass/Fail       |
| 7           | TC07             | Verify price updates with quantity change         | 1 litre = ₹50; select 2 litres                                                    | Total price should update to ₹100                                   | As per test       | Pass/Fail       |
| 8           | TC08             | Verify discount calculation for bulk order        | Quantity: 10 litres (eligible for 10% discount)                                   | Total = ₹450 instead of ₹500                                        | As per test       | Pass/Fail       |
| 9           | TC09             | Verify delivery time estimation                   | Address: Mumbai, Time: 8 AM                                                       | Delivery time displayed (e.g., “Delivery by 10 AM”)                 | As per test       | Pass/Fail       |
| 10          | TC10             | Verify order summary after selection              | Selected 2 litres, ₹100                                                           | Order summary should show quantity, price, and total correctly      | As per test       | Pass/Fail       |
| 11          | TC11             | Verify logout functionality                       | Click Logout button                                                               | User should be logged out and redirected to Login screen            | As per test       | Pass/Fail       |
| 12          | TC12             | Verify application handles invalid quantity input | Quantity entered: -5                                                              | Error message “Invalid quantity” should appear                      | As per test       | Pass/Fail       |
