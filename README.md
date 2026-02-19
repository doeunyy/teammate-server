# ⚾️ Teammate: Team Sports Matching & Venue Reservation Platform

> ### **TL;DR**
> - Built a **backend web service** for team sports matching and venue reservation
> - Designed a **relational database schema (ERD)** and implemented models using **MySQL + Sequelize**
> - Developed **RESTful APIs** for recruitment, approval workflows, and venue postings
> - Deployed a **containerized Node.js service** on **AWS Elastic Beanstalk** using Docker

<br>

This repository contains the **backend implementation of Teammate**, a web service designed to support sports clubs and communities by simplifying **team matching and game venue coordination**.  
The project focuses on building a scalable and maintainable backend system using a clean MVC architecture, well-defined REST APIs, and production-oriented deployment practices.

Teammate was developed as a team project within **UMC Ewha**, with an emphasis on **real-world backend engineering workflows**, including database modeling, API documentation, and cross-functional collaboration.

---

## Table of Contents
1. [Overview](#overview)
2. [Project Timeline](#project-timeline)
3. [Key Features](#key-features)
4. [System Architecture](#system-architecture)
5. [Implementation Details](#implementation-details)
6. [API Design](#api-design)
7. [Deployment](#deployment)

---

## Overview

Teammate addresses common challenges faced by amateur sports teams and clubs, such as:
- Finding opponent teams for matches
- Recruiting players for upcoming games
- Securing and sharing information about available sports venues

The platform provides structured workflows for **team recruitment, participation approval, and venue posting**, enabling users to coordinate games more efficiently through a centralized service.

This repository focuses exclusively on the **server-side implementation**, handling data persistence, business logic, and API communication with the frontend.



## Project Timeline
**Jan–Feb 2024 (5 weeks)**

| Week | Focus & Milestones |
|-----:|--------------------|
| 1 | Requirement analysis, feature definition, ERD design |
| 2 | Database schema implementation, Sequelize model setup |
| 3 | Core CRUD API development (recruitment, approval, venue) |
| 4 | API testing with Postman, error handling, refactoring |
| 5 | Dockerization, AWS Elastic Beanstalk deployment, documentation |


## Key Features
- Team recruitment posting and management
- Player participation request and approval workflows
- Sports venue posting and retrieval
- RESTful CRUD APIs with clear resource separation
- Centralized error handling and request validation
- API documentation for frontend collaboration


## System Architecture
```
Client (Web / Mobile)
↓
REST API (Express.js)
↓
Controller Layer
↓
Service / Business Logic
↓
Sequelize ORM
↓
MySQL Database
```


The backend follows a **layered MVC-style architecture**, separating routing, business logic, and data access to improve maintainability and scalability.

### Database Schema (ERD)

<img width="2450" height="1802" alt="Teammate-db" src="https://github.com/user-attachments/assets/3d9f0ac6-93da-4e58-b84d-8dd8e65c958d" />


The database schema was designed to support core workflows such as team recruitment, participation approval, venue posting, and user profile management, with normalized relations and clear ownership boundaries.

## Implementation Details

### Tech Stack
- **Language**: TypeScript
- **Runtime**: Node.js
- **Framework**: Express
- **Database**: MySQL
- **ORM**: Sequelize
- **Infrastructure**: Docker, AWS Elastic Beanstalk
- **Tooling**: Babel, Postman


### Database Design
- Designed a normalized **ERD** to model users, teams, recruitment posts, approvals, and venues
- Implemented relational constraints and associations using Sequelize
- Optimized query patterns for common access flows


## API Design
- RESTful endpoint structure following resource-based naming conventions
- CRUD APIs implemented for:
  - Recruitment posts
  - Participation requests and approvals
  - Venue postings
- Request validation and centralized error handling
- APIs tested using **Postman**
- API specifications shared with frontend developers for smooth integration


## Deployment
- Containerized the backend service using **Docker**
- Deployed the application on **AWS Elastic Beanstalk**
- Configured environment variables for production
- Verified service stability and API availability after deployment


