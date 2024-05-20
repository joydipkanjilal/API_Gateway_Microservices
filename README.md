# A Simple Application using API Gateway with Microservices



## **Architectural Goals**

1. Scalability: The ability of the system to handle growth in workload without performance degradation.
2. Performance: Ensuring that the system responds to and processes information within acceptable time frames.
3. Availability: Creating a system that is consistently operational and accessible to end-users, with minimal downtime.
4. Reliability: Designing the system to function correctly and consistently over time, with the ability to recover from faults.
5. Maintainability: Creating an architecture that allows for easy updates and maintenance without significant downtime or cost.
6. Security: Ensuring that the system is protected against unauthorized access, data breaches, and other security threats.
7. Testability: Designing the system such that it can be easily tested to verify its functionality.
8. Flexibility: The system should be able to adapt to changes without requiring much effort.
9. Usability: Ensuring that the system is user-friendly and intuitive to the target audience, reducing the learning curve.
10. Cost-effectiveness: The architecture should consider overall costs, including development, deployment, and maintenance, without compromising quality.
11. Interoperability: The ability of the system to work with other systems, leveraging APIs or data exchange protocols.
12. Portability: The system should be executable across different environments and platforms with minimal changes.

 

## **Architectural Constraints**

1. Technology stack limitations: The chosen technologies (programming languages, frameworks, databases) may impose constraints on what can be achieved or how it can be achieved.
2. Budget: Financial constraints that limit the resources available for implementing and maintaining the system.
3. Timeframe: Projects often have fixed deadlines requiring trade-offs to deliver on time.
4. Operational constraints: Operating systems, hardware specifications, and dependencies on external services.
5. Legacy systems: Existing infrastructure or systems that must be integrated or maintained can limit architectural options.
6. Resource availability: Limitations on human resources (expertise, number of developers) as well as physical resources (servers, data centers).
7. Vendor lock-in risks: Dependence on third-party vendors' platforms and technologies may influence architecture decisions in terms of flexibility and portability.
8. Network Latency: Microservices communicate over the network, which can introduce latency. 
9. Data Consistency: Each microservice is responsible for its own data persistence, leading to challenges in maintaining data consistency across services.
10. Security Concerns: There might be multiple points of potential security vulnerabilities which would require a comprehensive security strategy such as, implementing robust authentication, authorization, and encryption mechanisms.

 

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
