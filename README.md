# The airbnb clone project
An application project designed to simulate the development of a robust booking platform like Airbnb. It involves a deep dive into full-stack development, 
focusing on backend systems, database design, API development, and application security.

## Team Roles
- Backend Developer
- Database Administrator
- DevOps Engineer
- QA Engineer
- Frontend Developer
- UI/UX Designer

## Technology Stack
- Django: Python Web framework for building Restful API's. Provides Django REST Framework for creating and managing restful API's.
- PostgreSql: Relational database for data storage.
- GraphQL: Allows for flexible and efficient querying of data.
- Celery: For handling asynchronous tasks such as sending notifications or processing payments.
- Redis: Used for caching and session management.
- Docker: Containerization tool for consistent development and deployment environments.
- CI/CD Pipeline: Automated pipelines for testing and deploying code changes.

## Database Design
- Users
  - Username
  - Email
  - National ID NO.
- Property
  - Name
  - Location
  - Cost
  - Vacancy
- Payments
  - User
  - Property
  - Amount
  - Time
- Booking
  - User
  - Property
  - Period
  - Payment
- Review
  - Property
  - User
  - Rating
  - Description

- A user relates to a payment they make.
- A user relates to a booking they make.
- A user relates to a review they give
- A Property relates to a payment, booking and a review given.
  
## Feature Breakdown
- User management
  Manage users and their activities, from registration to user profile setting, recommendations, favourites.
- Properties management
  Manage details and activities related to Properties. 
  List Properties with their characteristics, cost, description, location and availability.
- Booking System
  Implement the booking of a room/house.
  After one sees the listings and identifies one they like, they can proceed to booking and checkout.
  This will also implement the payment as one books at checkout.

## API Security
- Authentication: username and password authentication, use of jwt tokens to authenticate resourse access.
- Authorization: role based authorization
- Rate limiting and Throttling: limit No. of requests to about 100 requests per minute per ip to protect against abuse and denial-of-service (DoS) attacks.

  Security is crucial for each area of the project since it is crucial to protect data, prevent abuse, and ensure only authorized access.

## CI/CD Pipeline
   Continuous Integration and Continuous Deployment/Delivery is crucial to ensure code is automatically build and tested every time changes are pushed to the repository and also automatic deployment of tested code to production or staging environments.
   This is crucial for faster deployments, Consistency and Reliability and Ealy Bug detection.
   CI/CD Tools that we'll use are:
   - Github Actions
   - Docker
   - Kubernetes

  

