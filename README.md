# Application Gateway - System Design POC

## Overview
An **Application Gateway** is a reverse proxy designed to route traffic to the appropriate backend service based on the application's configuration. It typically handles web traffic for multiple applications, offering features such as load balancing, security, and SSL termination.

## Key Concepts
- **Routing**: Application Gateway directs traffic to various backend services based on specific rules.
- **SSL Termination**: Encrypts/decrypts incoming traffic, offloading the backend services from handling encryption.
- **Load Balancing**: Distributes traffic across multiple instances of backend services to ensure high availability.

## Architecture Diagram
![Architecture Diagram](architecture-diagram.png)

## Use Cases
- **Microservices Communication**: Application Gateway as an entry point to route requests to different microservices based on paths.
- **Security**: Protects internal services by terminating SSL and handling DDoS mitigation.

## Implementation
The example code demonstrates setting up a basic Application Gateway with **[Visual Studio/.NET, C#]** and configures routing for multiple backend services.

### Example Code:
```bash
# Sample bash script for configuring the Application Gateway
$ gateway configure --backend service1 --path /service1
