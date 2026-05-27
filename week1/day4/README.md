# Day 4 - Salesforce Flow Builder

# 1. What is Flow Builder?

Flow Builder is a Salesforce automation tool used to automate business processes without writing code.

It helps companies:
- Reduce manual work
- Automate repetitive tasks
- Improve accuracy
- Increase productivity
- Build workflows visually

Flow Builder allows users to create automation using drag-and-drop elements.

---

# 2. Types of Flows

## Screen Flow

Screen Flow interacts with users through screens.

### Uses
- Data entry forms
- Step-by-step processes
- User input collection

### Example
Student registration form.

---

## Record-Triggered Flow

Record-Triggered Flow runs automatically when a record is created, updated, or deleted.

### Uses
- Automatic updates
- Notifications
- Business process automation

### Example
Automatically send an email when a student registers for a course.

---

# 3. Automation Ideas for College Management System

## 1. Auto Email After Student Registration

### Automation
Automatically send a confirmation email after student registration.

### Why Automation Helps
Saves staff time and ensures every student receives confirmation immediately.

---

## 2. Auto Update Remaining Seats

### Automation
Automatically decrease available seats when a student enrolls.

### Why Automation Helps
Prevents manual counting mistakes and keeps seat availability accurate.

---

## 3. Notify Faculty When Course Is Full

### Automation
Automatically notify faculty when course capacity is reached.

### Why Automation Helps
Helps faculty manage course planning efficiently.

---

## 4. Generate Student ID Automatically

### Automation
Automatically create a student ID during registration.

### Why Automation Helps
Avoids duplicate IDs and reduces manual effort.

---

## 5. Send Fee Payment Reminder

### Automation
Automatically send reminders before fee due dates.

### Why Automation Helps
Improves payment tracking and reduces delayed payments.

---

# 4. Flow Design Thinking

## Selected Process
Auto Email After Student Registration

---

# Simple Flow Diagram

```text
Start
   ↓
Student Record Created
   ↓
Check Student Email Exists?
   ↓
Yes ----------------→ Send Confirmation Email
   ↓
Update Registration Status
   ↓
End
```

---

# 5. Manual vs Automated Process

## Process Chosen
Student Course Registration

---

## Manual Process

1. Student fills registration form manually.
2. Staff verifies details.
3. Staff checks available seats.
4. Staff updates records manually.
5. Confirmation email is sent manually.

### Problems in Manual Process
- Time consuming
- Human errors
- Delayed communication
- Incorrect seat counts
- Higher workload for staff

---

## Automated Process Using Salesforce

1. Student submits registration form.
2. Salesforce Flow automatically checks seat availability.
3. Records are updated automatically.
4. Remaining seats are recalculated.
5. Confirmation email is sent instantly.

### Benefits of Automation
- Faster processing
- Accurate data
- Reduced manual work
- Better student experience
- Improved productivity

---

# 6. Reflection - Why Automation Matters in Enterprise Systems

Companies automate repetitive business processes to save time, improve accuracy, and reduce human errors.

Automation helps organizations:
- Increase productivity
- Maintain consistency
- Improve customer experience
- Reduce operational costs
- Speed up business workflows

Salesforce automation allows businesses to create efficient systems without heavy coding.

---

# 7. Reflective Questions

## 1. Why do companies automate workflows?

Companies automate workflows to save time, reduce manual work, and improve efficiency.

---

## 2. What problems happen with manual processes?

Manual processes can cause:
- Delays
- Human errors
- Duplicate work
- Inconsistent data
- Increased workload

---

## 3. Difference between Screen Flow and Record Triggered Flow?

| Screen Flow | Record Triggered Flow |
|---|---|
| Requires user interaction | Runs automatically |
| Used for forms and inputs | Used for automation |
| User starts the process | Salesforce starts the process |

---

## 4. Why is no-code automation powerful?

No-code automation allows businesses to automate processes quickly without requiring programming knowledge.

---

## 5. When should automation be avoided?

Automation should be avoided when:
- Human approval is necessary
- Processes change frequently
- Complex decision-making is required

---

## 6. How does automation improve consistency and productivity?

Automation performs tasks the same way every time, reducing mistakes and increasing speed and productivity.

---

# 8. Screenshots from Trailhead

## Flow Builder Basics Badge
flow-builder-basics.png

---

## Data and Actions in Flows Badge
data-actions-flows.png
