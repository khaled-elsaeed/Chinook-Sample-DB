# Chnook-Sample-DB
The Chinook Database Schema Example project provides a demonstration of a relational database schema design using the well-known "Chinook" sample database. The Chinook database is widely used for showcasing relational database concepts and is frequently utilized for testing and educational purposes.

The purpose of this project is to showcase how data can be organized and related within tables, and to serve as a reference for designing a database schema. By studying the Chinook database schema, developers and database administrators can gain insights into proper schema design techniques and understand how tables can be structured and interconnected to store and retrieve data efficiently.

Main Tables and Relationships:
The project focuses on six main tables within the Chinook database:

Employees: Stores employee-related data such as employee ID, name, job title, hierarchy, birth date, hire date, and address. The table includes a primary key on the EmployeeId field.

Customers: Stores customer information including customer ID, name, company, contact details (phone and email), city, and address. The table includes a primary key on the CustomerId field.

Invoices: Stores invoice data, including invoice ID, customer ID, invoice date, billing address, and billing city. The table includes a primary key on the InvoiceId field and a foreign key relationship with the Customers table.

Artists: Stores information about artists, such as artist ID and name. The table includes a primary key on the ArtistId field.

Albums: Stores album details, including album ID, title, and artist ID. The table includes a primary key on the AlbumId field and a foreign key relationship with the Artists table.

Tracks: Stores track information, including track ID, name, album ID, and unit price. The table includes a primary key on the TrackId field and a foreign key relationship with the Albums table.

The relationships between the tables are as follows:

Each employee can support one or many customers (Employees -> Customers).
Each customer can have multiple invoices (Customers -> Invoices).
Each invoice can relate to one or more tracks (Invoices -> Tracks).
Each track belongs to a specific album (Tracks -> Albums).
Each album is associated with a particular artist (Albums -> Artists).
This project includes an entity-relationship diagram (ERD) visualizing the relationships between the six main tables. The ERD provides a clear representation of how the tables are structured and interconnected, allowing users to grasp the relationships at a glance.
