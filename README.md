# Library-Management-System-ERD

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

Reservation: Contains Reservation ID, User ID (Reader), ISBN (Book), reserve and retu
