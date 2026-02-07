# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: 

**Business Context:**  
The university database system is used to manage information about students, instructors, courses, departments, sections, classrooms, and scheduling.

**Requirements:**  
-Store details of students, instructors, and departments.

-Maintain course and section information.

-Track which instructor teaches each section.

-Track which students enroll in sections.

-Manage classroom and time slot scheduling.

-Maintain course prerequisite details.

### ER Diagram:

<img width="1440" height="919" alt="ER diagram" src="https://github.com/user-attachments/assets/5e55b913-6eaa-4ce1-aee1-122a3c6a9e28" />


### Entities and Attributes

1.Department

Department Name (Primary Key)
Building
Budget

2.Instructor

Instructor ID (Primary Key)
Name
Salary

3.Student

Student ID (Primary Key)
Name
Total Credit

4.Course

Course ID (Primary Key)
Title
Credits

5.Section

Section ID (Primary Key)
Semester
Year

6.Classroom

Building
Room Number
Capacity

7.Time Slot

Time Slot ID (Primary Key)
Slot Time
Start Time
End Time
Day

### Relationships and Constraints

1.Course – Department

Each course belongs to one department.
One department can offer many courses.
(One-to-Many relationship)

2.Instructor – Department

Each instructor works in one department.
One department can have many instructors.
(One-to-Many relationship)

3.Student – Department

Each student is associated with one department.
One department can have many students.
(One-to-Many relationship)

4.Instructor – Section (Teaches)

An instructor can teach multiple sections.
A section is taught by one instructor.
(One-to-Many relationship)

5.Student – Section (Takes)

A student can enroll in multiple sections.
A section can have many students.
(Many-to-Many relationship)

6.Course – Section

Each section is related to one course.
A course can have many sections.
(One-to-Many relationship)

7.Section – Classroom

Each section is conducted in one classroom.
A classroom can host multiple sections at different times.
(One-to-Many relationship)

8.Section – Time Slot

Each section is assigned one time slot.
One time slot can be used by multiple sections.
(One-to-Many relationship)

### Assumptions
-Each student belongs to only one department.

-Each instructor works in only one department.

-Each section is assigned to one classroom and one time slot.

-A student can enroll in multiple sections.

-A course can have multiple sections.

-Prerequisite courses must be completed before enrolling.

## RESULT

Thus, the ER diagram for the University Database System was successfully designed by identifying the entities, attributes, relationships, and constraints.
This ER diagram clearly represents the academic structure and helps in efficient database implementation.

# Scenario B: City Library Event & Book Lending System

**Business Context:**  
The Central Library wants to manage book lending and cultural events.

**Requirements:**  
- Members borrow books, with loan and return dates tracked.  
- Each book has title, author, and category.  
- Library organizes events; members can register.  
- Each event has one or more speakers/authors.  
- Rooms are booked for events and study.  
- Overdue fines apply for late returns.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_library.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

# Scenario C: Restaurant Table Reservation & Ordering

**Business Context:**  
A popular restaurant wants to manage reservations, orders, and billing.

**Requirements:**  
- Customers can reserve tables or walk in.  
- Each reservation includes date, time, and number of guests.  
- Customers place food orders linked to reservations.  
- Each order contains multiple dishes; dishes belong to categories (starter, main, dessert).  
- Bills generated per reservation, including food and service charges.  
- Waiters assigned to serve reservations.

### ER Diagram:
*Paste or attach your diagram here*  
![ER Diagram](er_diagram_restaurant.png)

### Entities and Attributes

| Entity | Attributes (PK, FK) | Notes |
|--------|--------------------|-------|
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |
|        |                    |       |

### Relationships and Constraints

| Relationship | Cardinality | Participation | Notes |
|--------------|------------|---------------|-------|
|              |            |               |       |
|              |            |               |       |
|              |            |               |       |

### Assumptions
- 
- 
- 

---

## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
