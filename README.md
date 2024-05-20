# A Simple Application using API Gateway with Microservices

## Solution Structure

The application you are going to build will comprise the following projects as part of a single Visual Studio solution:

- **API.Gateway project** - This project represents the API Gateway and is responsible for getting requests from the clients and invoking the microservices.
- **Customer.API project** - This project defines the classes and interfaces used to represent the customer microservice.
- **Product.API project** - This project defines the types used to represent the product microservice.


The Customer.API microservice project will comprise the following classes and interfaces:

- **Customer class** – This represents the customer entity class.
- **ICustomerRepository interface** – This represents the interface for the customer repository.
- **CustomerRepositoryclass** – This represents the customer repository class that implements the ICustomerRepository interface.
- **CustomerController class** – This class represents the API controller for the Customer microservice.


The Product.API microservice project will contain the following types:

- **Product class** – This class represents the product entity.
- **IProductRepository interface** – This represents the interface for the product repository.
- **ProductRepository class** – This is the product repository class that implements the IProductRepository interface.
- **ProductController class** – This represents the API controller class for the Product microservice.
