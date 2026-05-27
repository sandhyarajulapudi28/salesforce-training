# Day 3 - Salesforce Data Modeling

# 1. Difference Between App, Object, Record, and Field

| Concept | Meaning |
|---|---|
| App | A collection of tabs, objects, and tools designed for a specific business purpose |
| Object | A database table used to store data |
| Record | A single row or entry inside an object |
| Field | A specific piece of information stored inside a record |

## Example
- App → College Management App
- Object → Student
- Record → Student Record
- Field → Email

---

# 2. Standard vs Custom Objects

## Standard Objects

Standard objects are already provided by Salesforce.

### Examples
- Account
- Contact
- Opportunity

These are commonly used CRM objects.

---

## Custom Objects

Custom objects are created by users based on business requirements.

### Examples
- Student
- Faculty
- Course
- Department

Custom objects help organizations build their own systems inside Salesforce.

---

# 3. College Data Model

## Objects
- Student
- Faculty
- Course
- Department

---

## Relationships

| Parent Object | Child Object | Relationship Type |
|---|---|---|
| Course | Student | One-to-Many |
| Department | Faculty | One-to-Many |
| Department | Course | One-to-Many |

Lookup relationships are used to connect these objects.

---

# College Data Model Diagram

```text
Department
   |
   |----< Faculty
   |
   |----< Course
               |
               |----< Student
```

---

# 4. Formula Fields

## Full Name

This formula field combines the first name and last name automatically.

### Formula

```text
First_Name & " " & Last_Name
```

### Why Automatic?

It reduces manual work and avoids typing mistakes.

---

## Percentage

This formula field calculates the student percentage automatically.

### Formula

```text
(Obtained_Marks / Total_Marks) * 100
```

### Why Automatic?

It prevents calculation errors and saves time.

---

## Remaining Seats

This formula field calculates available seats automatically.

### Formula

```text
Total_Seats - Filled_Seats
```

### Why Automatic?

It helps manage admissions efficiently and prevents overbooking.

---

# 5. Validation Rules

## Email Cannot Be Empty

### Rule

```text
ISBLANK(Email)
```

### Prevents

Missing student or faculty contact information.

---

## Student Age Cannot Be Negative

### Rule

```text
Age < 0
```

### Prevents

Invalid student records and incorrect data entry.

---

## Course Seats Cannot Exceed Limit

### Rule

```text
Filled_Seats > Total_Seats
```

### Prevents

Overbooking of courses beyond available capacity.

---

# 6. Reflection - Why Structured Enterprise Data Matters

Companies need structured data because it improves organization, security, reporting, automation, and accuracy.

Structured data helps businesses:
- Organize information properly
- Maintain relationships between records
- Generate reports easily
- Improve security
- Reduce mistakes
- Automate business processes

Random spreadsheets can create duplicate, inconsistent, and difficult-to-manage data.

Salesforce helps businesses manage data in a structured and efficient way.

---

# 7. Reflective Questions

## 1. Why can’t companies manage everything using Excel sheets?

Excel sheets become difficult to manage when data grows large. They can create duplicate records, inconsistent data, and security problems.

---

## 2. Why are relationships important between objects?

Relationships connect related data and help businesses manage information efficiently.

---

## 3. What problems happen if data is inconsistent?

Inconsistent data can cause:
- Incorrect reports
- Duplicate records
- Confusion
- Poor business decisions

---

## 4. Why should repetitive calculations be automated?

Automation reduces manual work, saves time, and avoids calculation mistakes.

---

## 5. Why should invalid data be blocked early?

Blocking invalid data improves data quality and prevents future business problems.

---

## 6. Why is Salesforce called a metadata-driven platform?

Salesforce is called a metadata-driven platform because applications and customizations are built using metadata instead of changing the core code.

---

# 8. Screenshots from Trailhead

## Data Modeling Badge
![Data Modeling](data-modeling.png)

---

## Formulas and Validations Badge
![Formulas and Validations](formulas-validations.png)
