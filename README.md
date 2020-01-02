Create a tiny RESTful web service with the following business requirements:

## Application must expose REST API endpoints for the following functionality:

* create product (price, productType, color, size)
* calculate order price (Collection of products and quantities)  (should also save Order draft somewhere)
* list all Orders
* list all Orders by productType

## Service must perform operation validation according to the following rules and reject if:

* type + color + size already exists
* Order is empty or total price is less than 10
* N orders / second are received from a single country (essentially we want to limit number of orders coming from a country in * a given timeframe)

Service must perform origin country resolution using a web service and store country code together with the order draft.
Because network is unreliable and services tend to fail, let's agree on default country code - "US".

## Technical requirements:

* Application has to be written in PHP using Symfony framework.
* Application has to be dockerized.
* Application has to have tests

## What gets evaluated:

* Are business requirements fulfilled
* RESTful best practices
* Software design
* Quality of the code
* Are tests useful and green

Happy Coding!
