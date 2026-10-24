# Cookie Order System

An Oracle SQL database for **Cookie Delight**, a small homemade cookie shop. It replaces handwritten notes, chat apps and spreadsheets with one central database for customers, orders, inventory, payments and delivery. Built as a group project for **ICT502 Database Engineering** (Group 1, CDCS2302A, Faculty of Computer and Mathematical Sciences, UiTM).

## Problem
Orders, stock and sales were tracked by hand, which caused order mistakes, no real-time inventory, no customer insights and slow operations.

## Objectives
- Store and manage customer orders and product information in a database
- Automate order processing to reduce human error
- Track cookie inventory accurately
- Generate sales and customer behaviour reports with SQL queries
- Explore scalable database solutions that support business growth

## What's Inside
- `cookie_schema.sql`: creates the tables and sequences and inserts sample data
- `docs/`: the full project report (PDF), the ERD image and the editable ERD (draw.io)
- `screenshots/`: table structures, DML (insert, update) results, the 10 SQL queries (Q6 to Q10 and more), plus inheritance and recursive examples

## Database Design
Tables: `ADMIN`, `CUSTOMER`, `COOKIE`, `COOKIE_REVIEW`, `CUSTOMER_ORDER`, `ORDER_COOKIE`, `DELIVERY`, `PAYMENT` and `METHOD_PAY`, linked by primary and foreign keys. `ORDER_COOKIE` links orders to the cookies in them. See `docs/ERD.png` for the relationships and the data dictionary in the report.

## Queries
The report includes 10 queries, for example:
- Customers who have placed an order, and customers who never have
- Total cookies sold and the top 3 best-selling cookies
- Orders above RM50 and the highest single payment
- Average order amount per customer
- Orders with their delivery method and status
- Number of orders by payment method

## How to Run
1. Open **Oracle SQL Developer** and connect to your database.
2. Open `cookie_schema.sql` and run it as a script.
3. The file contains some repeated `CREATE` statements, so Oracle may report "name is already used by an existing object" for those. They are safe to ignore.
4. Check that the tables exist and try the queries from the report.

## Notes
All names, emails, phone numbers and passwords in the sample data are made up for demonstration.

## My Contribution
This was a shared group project, and the work was split evenly between my teammates and me. My part included:
- Writing SQL queries for the report (for example joins, aggregates and ranking queries on orders, cookies, customers and payments)
- Preparing the example screens for advanced topics such as inheritance and recursive queries
- Helping with other parts of the database and the report, such as the tables, sample data and documentation
