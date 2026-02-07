# ER Diagram Workshop – Submission Template

## Objective
To understand and apply ER modeling concepts by creating ER diagrams for real-world applications.

## Purpose
Gain hands-on experience in designing ER diagrams that represent database structure including entities, relationships, attributes, and constraints.

---

# Scenario A: City Fitness Club Management


**Business Context:**  

FlexiFit Gym wants a database to manage its members, trainers, and fitness programs.

**Requirements:**  

-Members register with name, membership type, and start date.
-Each member can join multiple programs (Yoga, Zumba, Weight Training).
-Trainers assigned to programs; a program may have multiple trainers.
-Members may book personal training sessions with trainers.
-Attendance recorded for each session.
-Payments tracked for memberships and sessions.

### ER Diagram:

<img width="699" height="602" alt="Screenshot (769)" src="https://github.com/user-attachments/assets/c98f282b-d592-4306-a5f1-2923af6d670e" />


### Entities and Attributes

| Entity            | Attributes (PK, FK)                                             | Notes                               |
|-------------------|-----------------------------------------------------------------|-------------------------------------|
| Member            | MemberID (PK), Name, MembershipType, StartDate                  | Gym member details                  |
| Program           | ProgramID (PK), ProgramName                                     | Fitness program details             |
| Trainer           | TrainerID (PK), Name, Specialization                            | Fitness trainer info                |
| Session           | SessionID (PK), SessionDate, SessionTime, Status                | Personal training session details   |
| Payment           | PaymentID (PK), MemberID (FK), Amount, PaymentDate, PaymentType | Financial transaction tracking      |
| Enrollment        | MemberID (FK, PK), ProgramID (FK, PK)                           | Links members to programs           |
| ProgramAssignment | TrainerID (FK, PK), ProgramID (FK, PK)                          | Links trainers to programs          |
| Booking           | MemberID (FK, PK), TrainerID (FK, PK), SessionID (FK, PK)       | Links members, trainers, sessions   |

### Relationships and Constraints


| Relationship                     | Cardinality | Participation                         | Notes                                                                 |
|----------------------------------|-------------|--------------------------------------|----------------------------------------------------------------------|
| Member ENROLLS IN Program        | M:N         | Total (Enrollment), Partial (Member, Program) | Members can join multiple programs; programs have multiple members.   |
| Trainer LEADS Program            | M:N         | Partial (Trainer), Total (Program)   | Trainers lead multiple programs; programs have multiple trainers.     |
| Member BOOKS Session WITH Trainer| M:N         | Partial (Member, Trainer), Total (Session) | Members book sessions with trainers; trainers conduct sessions.       |
| Member MAKES Payment             | 1:N         | Total (Payment), Partial (Member)    | Payments by a member; a member makes many payments.                  |



### Assumptions
- IDs are primary keys and unique.
- Junction tables resolve all M:N relationships.
- Session status covers attendance.
---



## Instructions for Students

1. Complete **all three scenarios** (A, B, C).  
2. Identify entities, relationships, and attributes for each.  
3. Draw ER diagrams using **draw.io / diagrams.net** or hand-drawn & scanned.  
4. Fill in all tables and assumptions for each scenario.  
5. Export the completed Markdown (with diagrams) as **a single PDF**
