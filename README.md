# Full-stack Test for candidates

We expect that the candidate create a Web API and a Web Client to consume and display API data.

## Web API Technical Requisites

The usage of the following are demanded
- Language C# Latest Version
- .Net Core Latest Version
- Sql Server

## Web Client Technical Requisites
The implementation of the front-end must be separated from the Web API Solution and you are free to choose the tools used in the implementation

> 1. Create a register/login component
> 2. Create a component to add/update product
> 3. Create a orders component containing
>  * `Search` - Fields to filter orders by a interval of price and interval of creation date
>  * `List` - A list of orders. User must be able to click in a row to expand and see order details.

## WEB API Main Tasks

> 1. Create the following unauthenticated service endpoints
>  * `/signin` - *POST* - receiving an user name and a password
>  * `/signup` - *POST* - receiving an user full display name, an user name, a password and an e-mail address. Upon save time, add the current date and time to the database. An unique id must be created and used throughout the `/order/` POST endpoint described later in this document

> 2. Create the following authenticated service endpoints
>  * `/products` - *POST* - insert a new product to the product table with the following fields: id, name, description, price, creation date
>  * `/products/{id}` - *PUT* - update all passed fields in its appropriate record
>  * `/orders` - *POST* - inserts an order receiving an user id and a list of products id with the current price and quantity
>  * `/orders` - *GET* - returns all orders from the logged user. The search must accept optional filters by price range and date interval of creation date
>  * `/orders/{orderId}` - *GET* - returns details from a specific order. Details are the total value of the order and a list of products with their individual quantity and the price

## Services Requisites
- All endpoints must have automated tests that will prove the requisites are implemented
- Use as many design patterns and best practices as you see fit
- Use async methods anywhere you find it is needed
- ORM is open to your choice

## Database Requisites
- You are the responsible the create the database structure as best as you can think of. Conciseness, coherence and best practices are going to be considered

## Documentation Requisites
- It can be done in portuguese although being in english, french or spanish will also be considered a plus
- Should be easy to read and understand the usage (from a client developer's perspective) of your services
- It should be  easy to undertand how to execute your tests

## Last Requisites
- You can use your Github, GitLab or BitBucket to deliver this test
- You can fork from here to get started
- Try to keep your commits to a reasonable atomic capacity
- Use as much best practices you see fit to address the commits and/or branch naming

Feel free to ask me (*Luiz Roberto Rodolpho* - **luiz@portaltelemedicina.com.br**) any question.

You have 7 days counting from tomorrow to finish and deliver us the address of your github repository. Please, let us know if you need more time.



*Thank you for giving us this opportunity to get to know you and your work.*
