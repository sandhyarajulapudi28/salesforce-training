# Day 6 - SOQL and Apex Triggers

# 1. What is SOQL?

SOQL (Salesforce Object Query Language) is a query language used in Salesforce to retrieve data from objects.

It is similar to SQL but designed specifically for Salesforce data.

SOQL helps developers:
- Retrieve records
- Filter data
- Access related objects
- Search business information

---

# Example SOQL Query

```text
SELECT Name FROM Student__c
```

This query retrieves student names from the Student object.

---

# 2. What is an Apex Trigger?

An Apex Trigger is a piece of Apex code that automatically executes when specific events happen on Salesforce records.

Triggers run:
- Before insert
- After insert
- Before update
- After update
- Before delete
- After delete

Triggers help automate event-driven business logic.

---

# 3. Difference Between Flow and Trigger

| Flow | Apex Trigger |
|---|---|
| No-code automation tool | Code-based automation |
| Easier to build | More powerful and flexible |
| Best for simple processes | Best for complex logic |
| Uses drag-and-drop interface | Uses Apex programming |
| Faster development | Better for advanced automation |

---

# Difference Between Before Trigger and After Trigger

| Before Trigger | After Trigger |
|---|---|
| Runs before data is saved | Runs after data is saved |
| Used for validations and updates | Used for notifications and related actions |
| Can modify record values directly | Cannot change same record directly |

---

# 4. Trigger Use Cases in College Management System

## 1. After Student Registration → Send Welcome Email

### Trigger Event
After Insert on Student object

### Why?
Automatically welcomes newly registered students.

---

## 2. After Course Becomes Full → Notify Faculty

### Trigger Event
After Update on Course object

### Why?
Faculty should know when course capacity is reached.

---

## 3. After Attendance Drops Below 75% → Send Warning

### Trigger Event
After Update on Student Attendance

### Why?
Helps students improve attendance before exams.

---

## 4. After Fee Payment → Update Student Status

### Trigger Event
After Update on Fee record

### Why?
Automatically changes fee status to "Paid".

---

## 5. After Student Record Deletion → Archive Details

### Trigger Event
Before Delete on Student object

### Why?
Prevents accidental loss of important student information.

---

# 5. Flow vs Trigger Thinking

## Simple Email Notification

### Recommended
Flow

### Why?
Easy automation without coding.

---

## Complex Fee Eligibility Check

### Recommended
Apex Trigger

### Why?
Requires advanced calculations and multiple conditions.

---

## Updating Related Records

### Recommended
Flow

### Why?
Simple relationship updates can be handled easily using Flow.

---

## External API Integration

### Recommended
Apex Trigger

### Why?
External system communication requires custom programming.

---

# 6. Query Thinking Examples

## Find all students in Course A

```text
Retrieve all student records enrolled in Course A.
```

---

## Find all courses handled by Faculty X

```text
Retrieve all courses assigned to Faculty X.
```

---

## Find students with attendance below 75%

```text
Retrieve students whose attendance percentage is less than 75%.
```

---

## Find courses with available seats

```text
Retrieve all courses where remaining seats are greater than zero.
```

---

## Find students who did not pay fees

```text
Retrieve all students whose fee status is unpaid.
```

---

# 7. Reflection - Why Enterprise Systems Need Event-Driven Behavior

Enterprise systems manage large amounts of data and business activities continuously.

Event-driven behavior allows systems to:
- React automatically to changes
- Reduce manual work
- Improve speed and accuracy
- Send instant notifications
- Maintain data consistency

For example:
- When a student registers, confirmation emails can be sent automatically.
- When attendance becomes low, warning alerts can be triggered instantly.

Event-driven systems help businesses operate efficiently and respond quickly to important events.

---

# 8. Reflective Questions

## 1. Why do systems need triggers?

Triggers help systems respond automatically when data changes occur.

---

## 2. Difference between polling and event-driven systems?

| Polling | Event-Driven |
|---|---|
| Continuously checks for updates | Reacts only when events happen |
| Slower and less efficient | Faster and more efficient |
| Wastes resources | Saves resources |

---

## 3. Why are database queries important?

Queries help retrieve specific information quickly from large databases.

---

## 4. When should Flows be preferred over Triggers?

Flows should be preferred for simple automation because they are easier to build and maintain.

---

## 5. What problems happen if automation logic becomes too complex?

Complex automation can become difficult to maintain, debug, and understand.

---

## 6. Why should developers think carefully before automating actions?

Poor automation design can create incorrect updates, duplicate actions, and business problems.

---

# 9. Screenshots from Trailhead

## Database & .NET Basics
database-dotnet-basics.png

---

## Apex Triggers Badge
apex-triggers.png
