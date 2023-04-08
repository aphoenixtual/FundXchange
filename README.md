# CitiBank With Java Spring Boot Microservices

### Microservices Inside This Project

Here this project consist of mainly 6 microservices and those are,

- User service (banking-core-user-service) – This service includes all the operations under the User such as registrations and retrieval. Additionally, this API consumes keycloak REST API to register and manage the user base while using the local PostgreSQL database as well.
- Fund transfer service (banking-core-fund-transfer-service) – This is the service that handles all the fund transfers between accounts and this API will push messages to a centralized RabbitMQ queue to use from the Notification service.
- Payment service (banking-core-payments-service) – This service will include all the API endpoints to process Utility payments in this project and that will push notification messages to RabbitMQ as well.
- Notification service – This API is registered under the service registry but consumes all the messages from RabbitMQ and pushes necessary notifications to the end users.
- Banking core service – This is the banking core service that acts as a dummy banking core with accounts, users, transaction details, and processors for banking transactions.

### Base Project Architecture

<a href="#" target="blank">
    <img align="center" src="https://javatodev.com/content/images/wordpress/2021/05/Microservices-Article-Banking-Core-Concept-1024x870.png" 
alt="Spring Boot Microservices Project Architecture By Javatodev.com"/></a>

### Technology Stack

1. Java 11
2. Spring Boot 2.4.5
3. Netflix Eureka Service Registry
4. Netflix Eureka Service Client
5. Spring Cloud API Gateway
6. Spring Cloud Config Server
7. Zipkin
8. Spring Cloud Sleuth
9. Open Feign
10. RabbitMQ
11. Prometheus
12. Jitpack
13. MySQL
14. Keycloak
15. Docker / Docker Compose
16. Kubernetes
17. Keycloak

#### Author

<h1 align="center">Hi 👋, I'm Aayush Patel</h1>
<h3 align="center">A Passionate Java Fullstack Developer </h3>

<p align="left"> <a href="https://twitter.com/ayushp10" target="blank"><img src="https://img.shields.io/twitter/follow/ayushp10?logo=twitter&style=for-the-badge" alt="ayushp10" /></a> </p>
