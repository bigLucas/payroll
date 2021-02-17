# Spring RESTful API with HATEOAS
## Purpose:
- Simple project following the steps of the official [guide](https://spring.io/guides/tutorials/rest/) of Spring.
- With HATEOAS (Hypermedia as the Engine of Application State) all responses have a `_links` property to supply dynamic links with actions.
- The main difference between a *REST API* and a *RESTful API* is the **HATEOAS** resource present in a *RESTful API*.

## How to run?
- At root of the project run: `mvn clean spring-boot:run`.
- Call the `http://localhost:8080/employees` route.

## Available routes:
### /employees
* GET `/employees` - see all employees
* POST `/employees` - create a new employee
* GET `/employees/{id}` - find a specific employee
* PUT `/employees/{id}` - update a specific employee
* DELETE `/employees/{id}` - delete a specific employee

### /orders
* GET `/orders` - see all orders
* GET `/orders/{id}` - find a specific order
* POST `/orders` - create a new order
* DELETE `/orders/{id}/cancel` -  delete a specific order making the status go to canceled
* PUT `/orders/{id}/complete` - update a specific order to complete status