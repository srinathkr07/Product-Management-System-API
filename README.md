# Product-Management-System-API
An Open API Specification (OAS) for Product Management System done for the final assignment during PayPal India's Value Added Program (VAP).

This API can be used for all kinds of products. The data is broken down into mainly three collections - product, store and user. Endpoints have been written to perform basic operations like GET, PUT, POST and DELETE.

Description for the API specification can be found here: 
- https://app.swaggerhub.com/apis-docs/srinathkr07/ProductManagementSystem/1.0.0

And, the API specification can be found here: 
- https://app.swaggerhub.com/apis/srinathkr07/ProductManagementSystem/1.0.0#/

## Endpoints

### product

| Endpoint | Request Method | Description |
| --- | --- | --- |
| /product | GET | To get the list of products |
| /product | POST | To add a new product to the list of products |
| /product/{id} | GET | To get product details based on Product ID |
| /product/{id} | PUT | To update the details of an existing product, based on Product ID |
| /product/{id} | DELETE | To delete a product based on Product ID |

### store

| Endpoint | Request Method | Description |
| --- | --- | --- |
| /store/order | POST | To place a product order |
| /store/order/{orderId} | GET | To find a product order details based on Order ID |
| /store/order/{orderId} | DELETE | To delete a product order details based on Order ID |

### user

| Endpoint | Request Method | Description |
| --- | --- | --- |
| /user | POST | To create a new user |
| /user/login | GET | For an existing user to login |
| /user/logout | GET | For a logged in user to logout |
| /user/{username} | GET | To get user details based on username |
| /user/{username} | PUT | To update the details of an existing user, based on username |
| /user/{username} | DELETE | To delete a user based on username |

## Models

### Product

| Detail | Datatype | Description |
| --- | --- | --- |
| PId | string | ID of the product |
| Name | string | Name of the product |
| DateOfManufacture | string($date) | Date of Manufacture of the product |
| Category | string | Categore to which the product belongs |
| Price | number | Price of the product |
| Status | Enum | Status of the product i.e Available and Sold |

### User

| Detail | Datatype | Description |
| --- | --- | --- |
| UId | string | ID of the user |
| Username | string | Username of the user's account |
| FirstName | string | First name of the user |
| LastName | string | Last name of the user |
| Email | string | Email of the user |
| Password | string | Password of the user's account |
| Phone | string | Phone number of the user |

### Order

| Detail | Datatype | Description |
| --- | --- | --- |
| OId | string | ID of the order |
| PId | string | ID of the product |
| UId | string | ID of the user |
| Quantity | number | Quantity of the product ordered |
| ShipDate | string($date) | Shipping date of the order |
| Status | Enum | Status of the order i.e. Placed, Approved and Delivered |
| Complete | boolean (default: false) |  Completion status of the order |
