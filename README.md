# maven-lab1

## Project Structure

The project consists of a parent module called `commandes` and three child modules:

- **services**: Manages the business logic and application services.
- **web**: Handles the web controllers and REST API endpoints.
- **start**: Acts as the startup module for the application.

### Module Breakdown

1. **commandes (Parent Project)**:
   - The main project (parent) is a Spring Boot application, which contains common configuration files and dependencies for all modules.
   - Each child module is set up under this parent project using Maven.

2. **services**:
   - This module is responsible for the business logic and core functionality of the application.
   - Contains service classes, data access objects (DAOs), and any other core components necessary for order management.

3. **web**:
   - Manages the controllers and API endpoints.
   - Contains classes responsible for handling HTTP requests and routing them to the appropriate services.
   - Depends on the `services` module to utilize business logic.

4. **start**:
   - The main entry point for the Spring Boot application.
   - This module is responsible for starting the application and loading all other modules.
   - Uses the `web` and `services` modules as dependencies to build a complete application.
