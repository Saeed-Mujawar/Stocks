<h1 align="center"> Stock </h1>

-   The Stock Controller is a part of the Doctor App project, implemented using the Spring Boot framework. It provides various endpoints to manage stocks and perform CRUD operations. 

>### Prerequisites

-   MySql
-   SpringBoot
-   Java
>### Data flow

In this project, we have four layers-

-   Controller - The controller layer handles the HTTP requests, translates the JSON parameter to object, and authenticates the request and transfer it to the business (service) layer. In short, it consists of views i.e., frontend part.
-   Service -The business layer handles all the business logic. It consists of service classes and uses services provided by data access layers.
-   Repository - This layer mainatains the mySQl-database thing on which CRUD operations are performed
-   Model - This layer consists basically the class level things- the various classes required for the project and these classes consists the attributes to be stored.



>### Endpoints

- GET /stock/type/{stockType} : Get stocks based on the specified stock type.
- GET /stock/abovePrice/price/{price}/lowerData/date/{date} : Get stocks above the specified price and lower than the specified date.
- GET /stock/cap/{capPercentage} : Get all stocks above the specified market cap percentage.
- POST /stock/ : Insert stocks into the system.
- PUT /stock/marketCap/{marketCap}/id/{id} : Update the market cap of a stock based on the specified ID.
- PUT /stock/type/id : Update the type of a stock based on the specified ID using a custom query.
- PUT /stock/{id} : Update a stock based on the specified ID.
- DELETE /stock/ownerCount/{count} : Remove stocks based on the specified owner count.


>### Project Summary
This Spring Boot project, known as the StockApp, focuses on managing stocks. It provides a RESTful API for various operations such as retrieving stocks based on type, filtering stocks by price and date, querying stocks above a market cap, inserting new stocks, updating stock properties, and deleting stocks based on owner count. The project utilizes the Spring Boot framework, allowing for efficient development and deployment of the application. It aims to simplify stock management and enhance productivity in the context of the StockApp.
