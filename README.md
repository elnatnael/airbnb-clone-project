# airbnb-clone-project
The Airbnb Clone Project is a comprehensive, real-world application designed to simulate the development of a robust booking platform like Airbnb. It involves a deep dive into full-stack development, focusing on backend systems, database design, API development, and application security. This project enables learners to understand complex architectures, workflows, and collaborative team dynamics while building a scalable web application.
##Team Roles
Business analyst (BA): A business analyst dives deep into a customer’s workflows and analyzes stakeholder feedback to help clients formulate their wants and align a customer’s vision with what a development team is producing.
Product owner (PO): Holding more responsibility for a product’s success than any other development team member, a product owner is a decision-maker.
Project manager (PM): A project manager is responsible for distributing tasks across team members, planning work activities, and updating project status.
UI/UX designer: A UI designer devises intuitive, easy-to-use, and eye-pleasing interfaces for a product, while the UX part stands for thinking out the entire journey of a user’s interaction with a product. Thus, A UX designer is involved in user research, persona development, information architecture design, wireframing, prototyping, and more.
Software architect: An architect is an expert-level software engineer who makes executive software design decisions on behalf of an app development team.
Software developer: A software developer does the actual job and codes an application. And just like an app features a front end and a back end, there are front-end and back-end developers.
Quality assurance (QA) engineer: The job of a quality assurance engineer is to verify whether an application meets the requirements, both functional and non-functional. Functional requirements define what an application should do, while non-functional requirements specify how it should do that. To verify both, QA specialists run various checks, followed by analyzing the test results and reporting on the application quality.
Test automation engineer: A test automation engineer is there to help you test faster and better. To enable that, they develop test automation scripts—small programs that provide reliable and continuous feedback on application quality without any human involvement.
DevOps engineer: Even in Agile environments, development and operations teams can be siloed. DevOps engineers serve as a link between the two teams, unifying and automating the software delivery process and helping strike a balance between introducing changes quickly and keeping an application stable.
##Technology Stack
Django:It is a high-level Python Web framework used for building RESTful API.
Django REST Framework: provides tools for creating and managing RESTful APIs.
PostgreSQL: A powerful relational database used for data storage.
GraphQL: Allows for flexible and efficient querying of data.
Celery: For handling asynchronous tasks such as sending notifications or processing payments. 
Redis: used for caching and session management.
Docker: A Containerization  tool for a consistent development and deployment environment.
CI/CD Pipelines: Automated pipelines for testing and deploying code changes.  
##Database Design
Key entities : 
  User: 1. Name 
        2. Age 
        3. ID
  Properties: 1. Title 
              2. Description
              3. Location
              4. price_per_night 
  Bookings: 1. Id
            2. user_id = Foreign key to the Users table (the guest).
            3. Property_id = Foreign key to the Properties table (what’s being booked).
            4. total_Price = Calculated based on price per night × number of nights.
  Reviews: 1. user_id 
           2. property_id
           3. booking_id = Foreign key to the Bookings table (to ensure only completed stays can be reviewed)
           4. rating = Numeric score (e.g., 1 to 5 stars) 
           5. comment
  Payments: 1. booking_id
            2. amount = 
            3. currency = E.g., USD, EUR
            4. Payment method = E.g., credit card, PayPal, Stripe, Apple Pay
            5. status = E.g., pending, completed, failed, refunded
##Feature Breakdown
  User management: It helps the  Airbnb clone project by securely handling registration, login, roles (guest or host), and user data. It ensures personalized experiences, protects sensitive information, and enables key features like bookings, reviews, and payments to be correctly linked to each user.
  Property management: It enables hosts to create, update, and manage their listings, including descriptions, pricing, availability, and images. It ensures guests can browse accurate and up-to-date property information, which is essential for successful bookings and user trust.
  Booking system: It enables guests to reserve available properties for specific dates. It manages availability, prevents double bookings, and connects users, properties, and payments to ensure a smooth reservation process.
  Payment Processing: Integrate a payment system to handle transactions and record payment details.
  Review System: Allow users to leave reviews and ratings for properties.
  Data Optimization: Ensure efficient data retrieval and storage through database optimizations.


