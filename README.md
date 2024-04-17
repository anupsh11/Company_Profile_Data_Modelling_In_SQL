## Enterprise Data Architecture: Company Profile Data Modelling

### Overview
The "Enterprise Data Architecture: Company Profile Data Modelling" project is dedicated to designing a robust data model for managing various aspects of a company's profile, including offices, employees, customers, orders, products, payments, and product lines. This data model aims to provide a structured framework for organizing and analyzing essential company data, facilitating efficient data management, reporting, and decision-making processes.

### Data Structure
The project includes the following tables, each capturing specific aspects of the company's profile:

#### Offices
officeCode (int),
office_city (varchar),
phone (varchar),
addressLine1 (varchar),
addressLine2 (varchar),
state (varchar),
country (varchar),
postalCode (varchar),
territory (varchar)

#### Employees
employeeNumber (varchar),
lastName (varchar),
firstName (varchar),
extension (varchar),
email (varchar),
officeCode (int),
reportsTo (varchar),
jobTitle (varchar)

#### Customers
customerNumber (int),
customerName (varchar),
contactLastName (varchar),
contactFirstName (varchar),
city (varchar),
state (varchar),
postalCode (varchar),
country (varchar),
salesRepEmployeeNumber (varchar),
creditLimit (int)

#### Orders
orderNumber (int),
orderDate (datetime),
requiredDate (datetime),
shippedDate (varchar),
status (varchar),
comments (varchar),
customerNumber (int)

#### Order Details
orderNumber (int),
productCode (varchar),
quantityOrdered (varchar),
priceEach (decimal),
orderLineNumber (int)

#### Payments
customerNumber (int),
checkNumber (varchar),
paymentDate (datetime),
amount (decimal)

#### Product Lines
productLine (varchar),
textDescription (varchar)

#### Products
productCode (varchar),
productName (varchar),
productLine (varchar),
productScale (varchar),
productVendor (varchar),
quantityInStock (varchar),
buyPrice (varchar),
MSRP (varchar)

### Key Features
- Comprehensive Data Model: The project encompasses a comprehensive data model that covers various aspects of the company's profile, including organizational structure, customer relationships, sales transactions, and product catalog.
- Relationships and Constraints: The data model establishes relationships between different entities and enforces referential integrity constraints to maintain data consistency.
- Optimized for Analysis: The data model is optimized for efficient data analysis, enabling users to derive meaningful insights from company profile data.
- Scalability and Flexibility: The data model is designed to be scalable and adaptable to accommodate evolving business requirements and data growth.
- Documentation and Guidelines: Detailed documentation accompanies the project, providing insights into the data model structure, relationships, and best practices for data management.

### Usage
- Clone this repository to your local environment.
- Set up your preferred database management system (e.g., MySQL, PostgreSQL).
- Execute the provided SQL scripts to create the data model and populate it with sample data.
- Explore the data model structure and relationships to gain a deeper understanding of the company's profile data management.

### Contributions
Contributions to enhance the data model, improve documentation, or address any issues are welcome! Feel free to fork this repository, make changes, and submit pull requests.






