# Netflix Clone — Microservices Architecture

A full-stack **Netflix Clone** project built with **.NET 8**, **React/Next.js**, and a **Microservices Architecture**.

This repository (`netflix-clone`) serves as the **main entry point** — providing documentation and orchestrating the system via **Docker Compose**. Each service is maintained in its **own repository**.

---

## Project Overview

The goal of this project is to simulate a scalable streaming platform inspired by Netflix, using modern backend and frontend technologies, following microservice design principles.

### Objectives

- Build a **distributed, event-driven** architecture.
- Learn **microservice communication** patterns (HTTP, gRPC, message broker).
- Enable **CI/CD** pipelines for each microservice independently.

---

## Services

Each service is a standalone repository with its own CI/CD pipeline:

| Service     | Description                        | Port | Repository                                                                                         |
| ----------- | ---------------------------------- | ---- | -------------------------------------------------------------------------------------------------- |
| `auth`      | Handles authentication & JWT       | 5001 | [github.com/Bentanik/netflix-clone-auth](https://github.com/Bentanik/netflix-clone-auth)           |
| `media`     | Handles movies, videos, images     | 5002 | [github.com/Bentanik/netflix-clone-media](https://github.com/Bentanik/netflix-clone-media)         |
| `billing`   | Handles payments and subscriptions | 5003 | [github.com/Bentanik/netflix-clone-billing](https://github.com/Bentanik/netflix-clone-billing)     |
| `notify`    | Notification service (email, push) | 5004 | [github.com/Bentanik/netflix-clone-notify](https://github.com/Bentanik/netflix-clone-notify)       |
| `recommend` | Movie recommendation engine        | 5005 | [github.com/Bentanik/netflix-clone-recommend](https://github.com/Bentanik/netflix-clone-recommend) |
| `shared`    | Shared libraries / DTOs            | -    | [github.com/Bentanik/netflix-clone-shared](https://github.com/Bentanik/netflix-clone-shared)       |
| `gateway`   | API Gateway / routing              | 5000 | [github.com/Bentanik/netflix-clone-gateway](https://github.com/Bentanik/netflix-clone-gateway)     |
| `web`       | Frontend (React/Next.js)           | 3000 | [github.com/Bentanik/netflix-clone-web](https://github.com/Bentanik/netflix-clone-web)             |

---
