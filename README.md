# Best Buy – Store Front


This is the customer-facing web application for the **Best Buy Cloud-Native Final Project**.

The Store Front allows customers to browse products and place orders.  
It is part of a microservices-based architecture deployed to **Azure Kubernetes Service (AKS)**.

This project is adapted from the **Algonquin Pet Store (On Steroids)** reference architecture
and has been rebranded and extended for the Best Buy final project in CST8915.

---

## Architecture Context

The Store Front communicates with the following backend services:
- **Product Service** – retrieves product information
- **Order Service** – submits customer orders
- **RabbitMQ** – asynchronous messaging between services

All services are deployed as containers and orchestrated using Kubernetes.

---

## Running the App Locally (Optional)

> ⚠️ Local execution is for development and testing only.  
> In production, this service runs inside Kubernetes (AKS).

### Prerequisites
- Node.js  
- Vue CLI  
- Docker  
- Docker Compose  

### Local Development

The Store Front depends on the Product Service, Order Service, and RabbitMQ.
A `docker-compose` setup can be used for local testing.

```bash
docker compose up
``
 
