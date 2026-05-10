# SOFTWARE ARCHITECTURE

## 1. Monolith vs. Microservice
### Monolith: 
The entire application (database, UI, and business logic) is built as a single, large unit. It is easy to manage in small projects, but challenging for large-scale ones because fixing or updating one part carries a higher risk of breaking the entire system.

### Microservice: 
The application is divided into small, independent, and interconnected services. For example, the login and payment systems are separate. This way, if one part crashes, it does not cause the entire system to fail.

## 2. Architecture Patterns: MVC and MVVM
### It is about how we organize the code.

### MVC (Model-View-Controller): The most classic pattern.
- **Model:** Data and database processes.
- **View:** The interface that the user sees.
- **Controller:** The bridge (e.g., It manages what happens when a user clicks a button).

### MVVM (Model-View-ViewModel): 
Especially popular in modern mobile and web applications (React, Flutter, etc.). ViewModel automates the synchronization between the 'View' and the 'Model'.

## 3. State Management
It is the application's current "memory." For example, login status, items in a cart, or dark mode settings are all parts of the 'state.' As applications grow, keeping this information consistent across every page becomes difficult. State Management ensures that this data remains synchronized throughout the entire application.

## 4. Layered Architecture (Controller-Service-Repository)
Separating code into layers based on their responsibilities. This is a standard in the professional world, especially in Java Spring and C# .NET.

- **Controller:** Handles requests from the outside world (e.g., "A user requested this page").
- **Service:** Where the business logic happens (e.g., "Is the user eligible to register?", "Is the password suitable?").
- **Repository:** Responsible only for database communication (e.g., "Save this data" or "Fetch this user").