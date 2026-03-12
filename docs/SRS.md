# Software Requirements Specification (SRS) for the Veterinary Management System 

## 1. Introduction

### 1.1 Purspose 

This document is created with the purpose to specifying  
and describing the functional and non-functional  
requirements of the Veterinary Management System.

It also explains the architecture of the project with a clear way  
and justifies why this architectural style was selected. Show 
the scope of the system. 

### 1.2 Intended Audience  

This document is accessible for developer than will want contribute with  
the project.  

### 1.3 Intended Use  

The idea with this document is explaind in details the software.

### 1.4 Product Scope

The scope of the Veterinary Management System is: 

* Store management (product, sales, inventory)
* Client management
* Pet management
* Employe management
* Services of pets

### 1.5 Definition and Acronyms  

In this part is defined all key terms, acronyms,  
and abbreviations used in this SRS.  
This will help eliminate any ambiguity and ensure that all  
parties easily understand the document.  

## 2. Overall Description

### 2.1 User Needs
* The employe use this software to manage
### 2.2 Assumptions and Dependencies


## 3 System Features and Requirements

### 3.1 Functional Requirements

#### 3.1.1 Authentication
FR-1 The system shall provide a Login interface with username and password.
FR-2 The system shall login with Google account.
FR-3 The system shall validate user credentials before granting access.
FR-4 The system shall restrict access to authenticated users only.
FR-5 The system shall implement role-based access control.
FR-6 The system shall allow an administrator to create new user accounts.
FR-7 The system shall allow an administrator to assign roles to users.
FR-8 The system shall restrict system functionalities based on user roles.
FR-9 The system shall provide a logout functionality for all users.
FR-10 The system shall provide password recovery and reset functionality.

#### 3.1.2 Product & Inventory Management
FR-11 The system shall allow authorized users to create products.
FR-12 The system shall allow authorized users to update product information.
FR-13 The system shall allow authorized users to delete products.
FR-14 The system shall display a list of available products.
FR-15 The system shall track product stock levels.
FR-16 The system shall prevent sales if stock is insufficient.
FR-17 The system shall automatically update inventory after each sale.
FR-18 The system shall allow users to search and filter products.
FR-19 The system shall allow bulk import/export of product data.

#### 3.1.3 Services of the veterinary
FR-20 The system shall display a list of available veterinary services.  
FR-21 The system shall allow assigning a service to a pet.  
FR-22 The system shall allow only one active service per pet at a time.  
FR-23 The system shall allow adding service details such as cost and duration.

#### 3.1.4 Sales Management  
FR-24 The system shall allow authorized users to register sales.  
FR-25 The system shall calculate the total amount of each sale including taxes or discounts.  
FR-26 The system shall store sales transaction records.  
FR-27 The system shall generate sales and inventory reports.  
FR-28 The system shall allow filtering sales by date, product, oer client. 

#### 3.1.5 Client & Pet Management
FR-29 The system shall allow users to register clients.  
FR-30 The system shall allow users to register pets associated with a client.  
FR-31 The system shall allow users to view a pet's basic information.  
FR-32 The system shall allow users to view their own account information.  
FR-33 The system shall allow users to update their own account information.  
FR-34 The system shall allow users to delete their own account with a soft delete.  
FR-35 The system shall allow clients to have more than one pet.  
RF-36 The system shall allow storing pet medical history.  
RF-37 The system shall allow scheduling appointments for pets.

#### 3.1.6 Cart System
FR-38 The system shall allow users to add products or services to the cart. 
FR-39 The system shall allow users to update quantity of a product or service in the cart.  
FR-40 The system shall allow users to remove quantity a product or service from the cart.  
RF-41 The system shall calculate the total price of all items in the cart.  
RF-42 The system shall persist the cart for the logged-in user until checkout.  
RF-43 The system shall notify users if a product is low in stock.
RF-44 The system shall allow applying discounts or promotional codes in the cart.



### 3.1.2 EARS format: "When [event], the system shall [response]"

### 3.1.3 Include Specification By Example or BDD format (e.g, Gherkin) 


### 3.2 Non-Functional Requirements

### 3.2.1 Performance Requirements  

NFR-1 The system shall be able to handle a minimum a 50 users on concurrent.  
NFR-2 The system shall respond to user requests within 2 seconds under normal operating conditions

### 3.2.2 Security Requirements

NFR-3 The system shall restrict access to authenticated users only.  
NFR-4 User passwords shall be stored using secure hashing algorithms.  
NFR-5 The system shall use HTTPS for secure communication in production environments.  
NFR-6 The system shall validate all user inputs on the server side to prevent malicious data submission.
NFR-7 The system may implement client-side validation using JavaScript to improve user experience.


### 3.2.3 Reliability Requirements  

NFR-8 The system shall maintain data consistency and prevent data loss during normal operations.
NFR-9 The system shall ensure that database transactions are completed successfully or rolled back in case of failure.


### 3.2.4 Maintainability Requirements
NFR-10 The system shall follow the MVC architectural pattern.  
NFR-11 The system shall be developed using object-oriented programming principles.  
NFR-12 The system codebase shall be organized and documented to facilitate future maintenance and extension.

### 3.2.5 Usability Requirements
NFR-13 The system shall provide a clear and intuitive user interface for veterinary staff.  
NFR-14 The system shall allow users to perform common operations (such as registering sales or managing products) in no more than three steps.

### 3.3 Interface Requirements

NFR-15 The system shall provide a web-based interface accessible through modern web browsers.  
NFR-16 The system shall support responsive design to allow usage on desktop and tablet devices.


## 4. Design Constraints

## 5. Database Requirements  

Main entities: 

User
Role
Product
Inventory
Sale
SaleItem
Client
Pet
Service
Appointment
Cart
CartItem
MedicalHistory



## 6. Preliminary Schedule and Budget


## 7. Appendices

### 7.1 Glossary

### 7.2 Use Cases and Diagrams
References gathered around the development, definitions of some specific term.
