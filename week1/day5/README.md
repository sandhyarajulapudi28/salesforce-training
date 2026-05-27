# Day 5 - Introduction to Apex

# 1. What is Apex?

Apex is a programming language developed by Salesforce for building custom business logic and automation inside the Salesforce platform.

It is used when:
- Flows are not enough
- Complex logic is required
- External system integration is needed
- Advanced automation is required

Apex is similar to Java and runs on Salesforce servers.

---

# 2. Difference Between Flow and Apex

| Flow | Apex |
|---|---|
| No-code or low-code tool | Programming language |
| Uses drag-and-drop interface | Uses written code |
| Easier for simple automation | Better for complex logic |
| Faster to build | More flexible and powerful |
| Best for standard processes | Best for advanced business requirements |

---

# Difference Between Configuration and Coding

| Configuration | Coding |
|---|---|
| Uses clicks and settings | Uses programming logic |
| Faster and easier | More customizable |
| Requires less technical knowledge | Requires programming skills |
| Suitable for common requirements | Suitable for complex requirements |

---

# 3. Real Examples Where Apex Is Needed

## 1. Complex Fee Calculation

### Example
Calculate student fees based on:
- Scholarship
- Attendance
- Hostel fee
- Course type
- Late fee penalties

### Why Apex Is Needed

The logic becomes too complex for normal Flow conditions and formulas.

---

## 2. Integration with External Payment System

### Example
Connect Salesforce with an online payment gateway.

### Why Apex Is Needed

External API integration requires custom programming and HTTP requests.

---

## 3. Advanced Student Eligibility Checking

### Example
Allow course registration only if:
- Attendance is above 75%
- Previous course is completed
- Fees are cleared
- Student passed prerequisite subjects

### Why Apex Is Needed

Multiple validations and conditions require advanced business logic.

---

# 4. Integrated College Management System Design

## CRM Process

The College Management System works like a CRM system that manages:
- Student admissions
- Course registrations
- Faculty management
- Notifications
- Fee tracking

---

# Objects Used

- Student
- Course
- Faculty
- Department

---

# Relationships

| Parent Object | Child Object | Relationship |
|---|---|---|
| Department | Faculty | One-to-Many |
| Department | Course | One-to-Many |
| Course | Student | One-to-Many |

Lookup relationships connect these objects.

---

# Validation Rules

## Email Required
Prevents saving student records without email.

## Age Cannot Be Negative
Stops invalid student data.

## Seats Cannot Exceed Limit
Prevents overbooking of courses.

---

# Formula Fields

## Full Name
Automatically combines first name and last name.

## Percentage
Automatically calculates student percentage.

## Remaining Seats
Automatically calculates available course seats.

---

# Flow Automation

## Automated Processes

- Send confirmation email after registration
- Auto update remaining seats
- Notify faculty when course is full
- Send fee reminders
- Generate student ID automatically

Flows reduce manual work and improve efficiency.

---

# Apex Business Logic

## Custom Apex Usage

Apex handles:
- Complex fee calculations
- External payment integration
- Advanced eligibility logic
- Bulk student processing
- Custom validations

Apex gives more flexibility than Flow.

---

# 5. Pseudocode Examples

## Example 1 - Seat Availability

```text
IF seats are full
THEN block student registration
ELSE allow registration
```

---

## Example 2 - Attendance Warning

```text
IF attendance < 75%
THEN send warning notification to student
```

---

## Example 3 - Fee Reminder

```text
IF fee due date is near
THEN send payment reminder email
```

---

## Example 4 - Scholarship Eligibility

```text
IF percentage > 90%
THEN apply scholarship discount
```

---

# 6. Reflection - Why Enterprise Systems Eventually Need Programming

Enterprise systems become very complex as businesses grow.

Clicks and configuration are useful for standard automation, but some requirements need:
- Advanced logic
- External integrations
- Complex calculations
- High performance processing
- Custom business rules

Programming with Apex allows developers to build flexible and scalable solutions that cannot always be achieved using only no-code tools.

Salesforce combines both declarative tools and programming to create powerful enterprise applications.

---

# 7. Reflective Questions

## 1. Why is Apex needed if Salesforce already has Flows?

Flows are good for simple automation, but Apex is needed for advanced logic, integrations, and complex business rules.

---

## 2. When should developers prefer no-code solutions?

Developers should prefer no-code solutions when requirements are simple, standard, and easy to maintain.

---

## 3. What problems require custom programming?

Problems requiring:
- Complex calculations
- API integrations
- Advanced validations
- Bulk processing
- Custom workflows

usually need programming.

---

## 4. Why is business logic important in enterprise systems?

Business logic ensures processes follow company rules and operate correctly.

---

## 5. Why should developers avoid unnecessary coding?

Too much custom code increases maintenance complexity and development time.

---

## 6. How does programming increase flexibility?

Programming allows developers to build customized solutions beyond standard platform capabilities.

---

# 8. Screenshots from Trailhead

## Apex & .NET Basics
apex-.NET-basics.png

---

## Apex Basics & Database
apex-basics-database.png
