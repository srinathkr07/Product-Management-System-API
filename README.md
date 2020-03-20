# Product-Management-System-API
An Open API Specification (OAS) for Product Management System done for the final assignment during PayPal India's Value Added Program (VAP).

This API can be used for all kinds of products. The data is broken down into mainly three collections - product, store and user. Endpoints have been written to perform basic operations like GET, PUT, POST and DELETE operations.

Description for the API specification can be found here: 
https://app.swaggerhub.com/apis-docs/srinathkr07/ProductManagementSystem/1.0.0

And, the API specification can be found here: 
https://app.swaggerhub.com/apis/srinathkr07/ProductManagementSystem/1.0.0#/

## Endpoints

### product
| /product | GET | To get the list of products |
| /product | POST | To add a new product to the list of products |
| /product/{id} | GET | To get product details based on Product ID |
| /product/{id} | PUT | To update the details of an existing product, based on Product ID |
| /product/{id} | DELETE | To delete a product based on Product ID |
