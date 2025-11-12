# STQA



Set B (STQA)
QUESTION 1: TEST PLAN (14 Marks)

Case Study: Online Admission and Registration System (OARS)

Test Plan (IEEE 829 Format)
Test Plan Point	Answer
1. Test Plan Identifier	TP_OARS_001
2. References	SRS Document for OARS v1.0, IEEE Std 829-2008, University Admission Policy Document
3. Introduction	The OARS is an online portal designed to handle the entire admission process digitally, including registration, document upload, and payment. The goal is to ensure seamless student admission and reduce manual errors.
4. Features to be Tested	- User registration and login
- Application form submission
- Document upload and validation
- Admission status tracking
- Payment through card/net banking
5. Approach	Both manual and automated testing will be performed. Functional testing will validate all use cases; non-functional testing will cover performance and security.
6. Environmental Needs	- Hardware: Laptop/Desktop
- OS: Windows/Linux
- Browser: Chrome/Edge
- Tools: Selenium, Postman, MySQL Workbench
7. Staffing & Training Needs	- 2 Test Engineers
- 1 Test Lead
- Training in Selenium and defect tracking using JIRA
8. Responsibilities	- Test Lead: Prepare test plan and review test cases
- Testers: Execute tests and log defects
- Developer: Fix defects
9. Schedule	Test Plan Prep: 12 Nov
Test Case Design: 13–14 Nov
Execution: 15–17 Nov
Bug Fix & Retest: 18–19 Nov
Final Report: 20 Nov
10. Approval	Approved by Project Manager and QA Head
QUESTION 2: TEST CASES (06 Marks)

Task: Write minimum 12 test cases for above case study

Test Cases for OARS System
Sr. No.	Test Case ID	Test Scenario / Step	Test Data	Expected Result	Actual Result	Pass / Fail
1	TC_OARS_01	Verify registration with valid details	Valid name, email, password	Registration successful	—	—
2	TC_OARS_02	Verify registration with existing email	Already registered email	Error “Email already exists”	—	—
3	TC_OARS_03	Verify login with valid credentials	Valid username/password	User logged in successfully	—	—
4	TC_OARS_04	Verify login with invalid password	Wrong password	Error “Invalid credentials”	—	—
5	TC_OARS_05	Verify application form submission	All fields filled correctly	Form submitted successfully	—	—
6	TC_OARS_06	Verify mandatory field validation	Missing required fields	Display error messages	—	—
7	TC_OARS_07	Verify document upload	Valid file type & size	Document uploaded successfully	—	—
8	TC_OARS_08	Verify invalid document upload	File >10MB or wrong format	Error “Invalid file type/size”	—	—
9	TC_OARS_09	Verify payment process	Valid card/net banking details	Payment successful message	—	—
10	TC_OARS_10	Verify status checking	Valid application ID	Status displayed correctly	—	—
11	TC_OARS_11	Verify logout functionality	Click on logout	Redirect to login page	—	—
12	TC_OARS_12	Verify system security	Attempt SQL injection	Input sanitized; error handled	—	—




Set A (STQA Assessment)
QUESTION 1: TEST PLAN (14 Marks)

Case Study: Cloud Kitchen Aggregator App

IEEE 829 Test Plan Format
Test Plan Point	Answer
1. Test Plan Identifier	TP_CKA_001
2. References	SRS Document v1.0 for Cloud Kitchen Aggregator App, IEEE Std 829-2008, API Integration Docs of Delivery & Payment Partners
3. Introduction	The Cloud Kitchen Aggregator App allows users to browse menus, place orders from partner kitchens, track delivery status, and make payments via integrated gateways. It also helps kitchens manage orders and promotions.
4. Features to be Tested	- User registration and login
- Browse menus and place orders
- Add/remove items from cart
- Payment via third-party gateway
- Order tracking with delivery status
- Kitchen dashboard for order management
- Promotional offers and notifications
5. Approach	Functional, integration, and system testing will be performed using a combination of manual and automation techniques. API testing will validate 3rd-party integration. Performance and security testing will also be executed.
6. Environmental Needs	- Hardware: Laptop/Desktop with 8 GB RAM
- Software: Windows/Linux, Chrome Browser
- Database: MySQL
- Tools: Postman, Selenium, JIRA for defect tracking
7. Staffing & Training Needs	1 Test Lead and 2 QA Engineers. Training in API testing, Selenium automation, and JIRA.
8. Responsibilities	- Test Lead: Prepare and review test plan, monitor progress
- Tester: Create and execute test cases, log defects
- Developer: Fix defects and support retesting
9. Schedule	Test Plan Preparation – 10 Nov
Test Case Design – 11–12 Nov
Execution – 13–15 Nov
Defect Fix & Retest – 16–17 Nov
Closure – 18 Nov
10. Approval	Approved by Project Manager and QA Lead before UAT execution.
QUESTION 2: TEST CASES (6 Marks)

Task: Write minimum 12 test cases for the above case study.

Test Cases for Cloud Kitchen Aggregator App
Sr No.	Test Case ID	Test Scenario / Step	Test Data	Expected Result	Actual Result	Pass/Fail
1	TC_CKA_01	Register user with valid details	Valid email, password	Account created successfully
2	TC_CKA_02	Register with existing email	Duplicate email	Error message displayed
3	TC_CKA_03	Login with valid credentials	Valid ID and password	Redirect to home dashboard
4	TC_CKA_04	Login with invalid password	Wrong password	Display error “Invalid credentials”
5	TC_CKA_05	Search for a kitchen by location	“Pune”	List of kitchens in Pune displayed
6	TC_CKA_06	Add item to cart	Select menu item	Item added to cart
7	TC_CKA_07	Remove item from cart	Click “remove”	Item removed successfully
8	TC_CKA_08	Place order with valid details	Valid address and payment	Order placed successfully
9	TC_CKA_09	Cancel order before dispatch	Valid order ID	Order status changed to “Cancelled”
10	TC_CKA_10	Check order status	Order ID	Shows “Preparing/Out for Delivery”
11	TC_CKA_11	Make payment via third-party gateway	Valid card details	Transaction success message
12	TC_CKA_12	Verify promo code discount	Valid coupon code	Discount applied on total amount
13	TC_CKA_13	Logout from app	Click logout	Redirect to login screen




Set C (STQA Assessment)
QUESTION 1: TEST PLAN (14 Marks)

Case Study: University Result Declaration System

IEEE 829 Test Plan Format
Test Plan Point	Answer
1. Test Plan Identifier	TP_URDS_001
2. References	SRS Document for University Result Declaration System v1.0, IEEE Std 829-2008, University Academic Policy for Result Publication & Revaluation
3. Introduction	The University Result Declaration System (URDS) provides students access to their results semester/year-wise. It enables downloading of scorecards and supports online application for rechecking/re-evaluation with integrated payment.
4. Features to be Tested	- Student login & authentication
- View results (semester/year-wise)
- Download result in PDF format
- Apply for rechecking/re-evaluation
- Online payment for re-evaluation
- Admin result upload & verification
- Email/SMS notifications to students
5. Approach	Testing will be done using manual and automated testing approaches. Functional testing will verify result viewing and application processes, while integration testing will check payment gateway and data synchronization. Security and usability tests will also be included.
6. Environmental Needs	- Hardware: Windows/Linux system with 8 GB RAM
- Software: Chrome, MySQL, Node.js server
- Tools: Selenium, Postman, JIRA for defect tracking
7. Staffing & Training Needs	- 1 Test Lead, 2 QA Testers
- Testers trained in database validation, payment gateway testing, and security validation.
8. Responsibilities	- Test Lead: Define plan, assign tasks, and review deliverables.
- Testers: Create, execute, and document test cases.
- Developers: Resolve bugs and support regression testing.
9. Schedule	Requirement Study: 12 Nov
Test Plan Preparation: 13 Nov
Test Case Development: 14–15 Nov
Execution: 16–18 Nov
Retesting: 19 Nov
Closure: 20 Nov
10. Approval	Approved by Project Manager and QA Head before release.
QUESTION 2: TEST CASES (06 Marks)

Task: Write minimum 12 test cases for the above system.

Test Cases for University Result Declaration System
Sr No.	Test Case ID	Test Scenario / Step	Test Data	Expected Result	Actual Result	Pass/Fail
1	TC_URDS_01	Verify student login with valid credentials	Valid Roll No & Password	Redirect to dashboard
2	TC_URDS_02	Verify login with invalid credentials	Wrong password	Show “Invalid Credentials”
3	TC_URDS_03	View results for selected semester	Sem = 4	Display all subject marks for Sem 4
4	TC_URDS_04	View results for selected academic year	Year = 2024	Show results for the chosen year
5	TC_URDS_05	Download result as PDF	Click “Download”	PDF downloaded successfully
6	TC_URDS_06	Apply for rechecking of one subject	Select subject = “DBMS”	Application submitted
7	TC_URDS_07	Apply for re-evaluation with payment	Valid payment details	Payment successful message
8	TC_URDS_08	Verify re-evaluation request appears in student dashboard	Valid Roll No	Application shows “Pending/Approved”
9	TC_URDS_09	Verify admin can upload result data	Admin credentials	Results uploaded successfully
10	TC_URDS_10	Verify system prevents duplicate re-evaluation requests	Duplicate request	Error “Request already exists”
11	TC_URDS_11	Validate email/SMS notification for result declaration	Result published	Notification sent to student
12	TC_URDS_12	Validate security session timeout	Idle > 15 min	Auto logout and redirect to login
