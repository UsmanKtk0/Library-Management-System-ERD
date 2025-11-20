# Library-Management-System-ERD

Library Management System ERD


# Overview
This project presents the Entity Relationship Diagram (ERD) for a Library Management System designed to model the data structure and relationships of a comprehensive library environment. The ERD was created using Canva and aims to provide a clear, organized visualization of key entities, their attributes, and how they interrelate within the system.



# Purpose
The ERD serves to capture all relevant data components needed to manage library operations including book cataloging, member management, staff oversight, reservations, fines, and reporting. It offers a blueprint for database design and implementation for efficient library management.




# Entities and Attributes
Library Branch: Identified by Branch ID, with attributes such as Name, Address, and linked Departments.

Department: Contains Department ID, Name, Manager ID, linked to Staff and Library Branches.

Book: Identified by ISBN, with attributes including Title, Author Name, Price, and Publisher ID.

Publisher: Maintains Publisher ID, Name, Year of Publication.

Staff: Identified by Staff ID, Name, Login ID, associated with Departments, and can manage Books and Reports.

Reader: Features User ID, personal details (Name split as First, Middle, Last), Email, and Phone Number.

Reservation: Contains Reservation ID, User ID (Reader), ISBN (Book), reserve and return dates, and status.

Fine: Maintains Fine ID, User ID, Amount, Date, and Reason.

Reports: Includes Report ID, User ID, ISBN, Title, and Staff ID.

System: Records Login ID, User Name, Password, linked to Staff for login management.






# Relationships
One Publisher can publish many Books (1:M).

Books can be maintained by multiple Staff members (M:N).

Books can be loaned by multiple Readers and vice versa (M:N).

Staff can manage multiple Reports and track multiple Readers (1:M and M:N respectively).

Readers can register multiple Reservations and pay multiple Fines (1:M).

Departments have multiple Staff members and belong to a Library Branch (1:M and M:1).

Staff have a hierarchical reporting structure via Manager ID (self-relationship).




# Additional Details
Primary keys and foreign keys have been defined for each entity to maintain integrity.

Cardinalities indicate the nature of relationships facilitating database normalization.

The ERD reflects a real-world library workflow accommodating user management, resource tracking, and administrative oversight.




# Tools and Design
The ERD was created using Canva for a clean, visually appealing presentation.
