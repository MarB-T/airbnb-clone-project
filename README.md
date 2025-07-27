# ALX Pro-Dev Learning project using Django
## About the Project
The Airbnb Clone Project is a comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb. It involves a deep dive into full-stack development, focusing on backend systems, database design, API development, and application security. This project enables learners to understand complex architectures, workflows, and collaborative team dynamics while building a scalable web application.
  
## Team Roles
### Business analyst (BA)
Understands and help define the customer's business needs aligning the customer's vision with the development team.
### Software developer
Develops the backend API and intergrations with the database
### UI/UX Designer
Designs and develops the UI and UX of the webapp/project
### Database Administrator
Designs and manages the database schemas, access, backups, etc
### Test engineer
Designs and automate tests ensuring all the edge cases are considerd and catered for.
### Product owner
Holds responsibility for a product vision and evolution. Holding more responsibility for a product’s success than any other development team member, a product owner is a decision-maker. Balancing both business needs and market trends, they define a business strategy, shape up the product vision, make sure it satisfies customer needs, and manage a product backlog.
### DevOps engineer
Facilitates cooperation between development and operations teams. Builds continuous integration and continuous delivery (CI/CD) pipelines for faster delivery.
  
## Technology stack
These are the technologies that will be used in the project
- Django: A web framework for developing the backend  RESTFUL APIs.
- PostgreSQL: The DBMS for the project's database.
- GraphQL: - A query language and runtime for executing queries, enabling the client side of the app to interact with the database.
- ReactJS: Used to develop the client side of the project.
  
## Database Design
An overview of the database
---
| Entity       | Description                                   | Fields                                        | 
|--------------|-----------------------------------------------|-----------------------------------------------|
| Users        | The users registered on the website           | Name, PhoneNumber, Age                        |
| Properties   | The list of properties registered on the site | Locattion, Size, Price                        |
| Bookings     | A register of bookings                        | Property. Date, Amount                        |

## Feature Breakdown
- Property management
- User management
- Property review
- Booking system
- Online payment

## API security
Securing backend APIs is critical in any web application, especially for a platform like an Airbnb clone that handles sensitive user data, bookings, messaging, and payments. Below are the key security measures we will implement and why they are crucial for the safety and integrity of the system.
### Authentication
Ensures only registered users can access protected areas
- Use JWT (JSON Web Tokens) or session-based authentication to validate users.
- Require login for actions like booking, listing, or messaging.
### Authorization
Controls what an authenticated user is allowed to do
- Role-based access: Admin vs. host vs. guests
- Ensure users can only update or delete their own listings or bookings
### Rate Limiting & Throttling
Limits how many requests a user can make in a specific timeframe
- Use Django REST Framework's throttling classes or NGINX-level rate limiting.
- Apply different rates for anonymous vs. authenticated users.
### Data Validation and Sanitization
Ensures incoming data is clean and conforms to expectations.
- Use serializers in Django REST Framework to validate incoming payloads.
- Strip malicious scripts and inputs
### HTTPS and Secure cookies
Encrypts data in transit and secures session cookies.
- Use HTTPS in production
- Set secure, httponly, and samesite flags for cookies
### Secure Payment Processing
Ensure safe handling of financial transactions
- Never store card information
- Use trusted gateways like Stripe, Draja or PayPal
### Logging and Monitoring
Track system behavior and detect suspicious activity
- Log failed logins, password changes, and critical actions
- Use tools like Sentry or Django Admin logs for monitoring

## CI/CD Pipeline
A set of practices that automate the process of building, testing, and deploying code.
### Tools that can be used
| Purpose           | Tool example                                         |
|-------------------|------------------------------------------------------|
| Version control   | Git + Github                                         |
| CI/CD Automation  | GitHub Actions, GitLab CI, CircleCI, Jenkins         |
| Deployment        | Render, Heroku, Vercel, Netlify, Docker+VPS          |
| Testing           | pytest,  Django Test Framework, Jest                 |
| Containerization  | Docker                                               |

---


