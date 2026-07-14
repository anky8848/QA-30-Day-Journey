# Day 2 – Software Development Life Cycle (SDLC)

## What is SDLC?

Software Development Life Cycle (SDLC) is a structured process used to design, develop, test, deploy, and maintain software efficiently. It helps teams deliver high-quality software within budget and on schedule.

---

# SDLC Phases

## 1. Requirement Gathering
- Understand client requirements.
- Gather business and functional requirements.
- QA reviews requirements to ensure they are clear and testable.

## 2. Planning
- Define project scope.
- Estimate budget and timeline.
- Allocate resources.

## 3. Design
- Create UI/UX designs.
- Design database and system architecture.
- QA reviews design for testability.

## 4. Development
- Developers write the application code.
- QA prepares test scenarios and test cases.

## 5. Testing
- QA executes test cases.
- Bugs are identified and reported.
- Developers fix bugs.
- QA performs retesting.

## 6. Deployment
- The tested application is released to the production environment for end users.

## 7. Maintenance
- Fix bugs reported by users.
- Improve performance.
- Add new features.
- Release security updates.

---

# QA's Role in SDLC

QA contributes throughout the SDLC, not only during testing.

- Review requirements.
- Review design documents.
- Prepare test scenarios.
- Create test cases.
- Execute tests.
- Report bugs.
- Retest fixed issues.
- Perform regression testing.
- Support production releases.

---

# Waterfall vs Agile

| Waterfall | Agile |
|------------|--------|
| Sequential process | Iterative process |
| Testing happens at the end | Testing happens continuously |
| Difficult to change requirements | Easy to accommodate changes |
| Slower feedback | Faster feedback |
| Less flexible | Highly flexible |

---

# Verification vs Validation

## Verification
- Are we building the product correctly?
- Performed before software execution.
- Reviews requirements, documents, and designs.

## Validation
- Are we building the right product?
- Performed by executing the software.
- Ensures the application meets user requirements.

---

# Key Learnings

- SDLC consists of seven phases.
- QA is involved from the requirement phase until maintenance.
- Agile is more flexible than Waterfall.
- Verification checks documents, while Validation checks the working software.





# Practical Analysis – SauceDemo & OrangeHRM

## Website 1 – SauceDemo

### Features Identified

1. User Login
2. Product Listing
3. Product Information Display
4. Add to Cart
5. Remove from Cart
6. Shopping Cart
7. Checkout
8. Product Sorting
9. About Page
10. Logout

---

### Possible Modules

1. Authentication Module
2. Product Catalog Module
3. Shopping Cart Module
4. Checkout Module
5. Product Details Module
6. Product Sorting Module
7. Navigation Module
8. User Session Module
9. About Module
10. Footer Module

---

### Testing Priority

1. Authentication (Login)
2. Product Display
3. Shopping Cart
4. Product Sorting
5. Checkout
6. Navigation
7. Logout

---

## Website 2 – OrangeHRM

### Features Identified

1. User Login
2. Password Management
3. Employee Search
4. Attendance Management
5. Timesheet Management
6. Project Management
7. Report Generation
8. Employee Profile Management
9. Dashboard Viewing
10. User Logout

---

### Modules

1. Admin
2. PIM
3. Leave
4. Time
5. Recruitment
6. My Info
7. Dashboard
8. Directory
9. Maintenance
10. Claim
11. Buzz

---

### Testing Priority

1. Authentication (Login)
2. Dashboard Loading
3. Employee Management (PIM)
4. Attendance (Punch In/Out)
5. Timesheets
6. Employee Search
7. Add Employee
8. Edit Employee
9. Delete Employee
10. Logout

---

# Observation

During this practical exercise, I learned to identify application features, understand software modules, and prioritize testing based on business impact. I also realized that QA engineers focus on critical functionality first, such as authentication, before testing other modules.










# Day 2 Interview Questions

## 1. What does SDLC stand for?

Software Development Life Cycle.

---

## 2. Which phase comes after Design?

Development (Coding).

---

## 3. In which phase is coding done?

Development Phase.

---

## 4. Who writes the code?

Software Developers.

---

## 5. What is Deployment?

Deployment is the process of releasing tested software to the production environment where end users can access and use it.

---

## 6. What is Maintenance?

Maintenance is the phase after deployment where bugs are fixed, new features are added, performance is improved, and security updates are released.

---

## 7. Verification or Validation: Checking a requirements document?

Verification.

---

## 8. Verification or Validation: Testing a login page?

Validation.

---

## 9. Which model is more flexible: Waterfall or Agile?

Agile, because it allows continuous development, testing, and easier adaptation to changing requirements.

---

## 10. Can QA contribute before coding starts?

Yes.

QA participates from the requirement and design phases by reviewing requirements, identifying ambiguities, preparing test scenarios, and writing test cases before development is completed.