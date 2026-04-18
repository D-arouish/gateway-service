# gateway-service

API gateway for the e-commerce microservices platform. This service sits at the edge of the system and is designed to route client requests to internal services discovered through Eureka.

## Responsibilities

- central entry point for backend APIs
- integrates with Eureka and the config server
- supports route configuration through Spring Cloud Gateway
- exposes actuator endpoints for monitoring

## Stack

- Java 17
- Spring Boot
- Spring Cloud Gateway
- Eureka Client
- Spring Cloud Config Client
- Spring Boot Actuator

## Notes

The repository includes an example `application.yml` showing how customer and product routes can be defined locally. In a full deployment, gateway configuration can also be externalized through the config server.

## Run Locally

```bash
./mvnw spring-boot:run
```
