# Full-stack Test for candidates

## Web API Technical Requisites

The usage of the following are demanded
- Language C# Latest Version
- .Net Core Latest Version
- Sql Server

## Main Tasks

> 1. Create the following unauthenticated service endpoints
>  * `/signin` - *POST* - receiving an user name and a password
>  * `/signup` - *POST* - receiving an user full display name, an user name, a password and an e-mail address. Upon save time, add the current date and time to the database. An unique id must be created and used throughout the `/order/` POST endpoint described later in this document

> 2. Create the following authenticated service endpoints
>  * `/products` - *POST* - insert a new product to the product table with the following fields: id, name, description, price, creation date
>  * `/products/{id}` - *PUT* - update all passed fields in its appropriate record
>  * `/orders` - *POST* - inserts an order receiving an user id and a list of products id with the current price and quantity
>  * `/orders` - *GET* - returns all orders from the logged user. The search must accept filters by price range and date interval of creation date.
>  * `/orders/{orderId}` - *GET* - returns details from a specific order. Details are the total value of the order and a list of products with their individual quantity and the price.
