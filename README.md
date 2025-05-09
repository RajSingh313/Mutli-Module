# Multi-Module Spring Boot Project

This is a Spring Boot project structured as a **multi-module Maven project** to promote modularity, code reuse, and better organization. It consists of two modules:

- `tracking-api-module`: The main Spring Boot application module.
- `specification-module`: A supporting module containing reusable specifications or logic.


## ✅ What Has Been Set Up

- **Parent POM (`mutlimodule/pom.xml`)**
  - Set packaging to `pom`
  - Declared both sub-modules
  - Defined common dependencies
  - Configured `spring-boot-maven-plugin` inside `pluginManagement` to avoid packaging conflicts

- **Main Module (`tracking-api-module`)**
  - Moved `MainApplication.java` and `resources/` from root into this module
  - Applied `spring-boot-maven-plugin` here only for packaging and running the Spring Boot application

- **Supporting Module (`specification-module`)**
  - Created as a standard Maven module, used to share code with other modules

## 🚀 Running the Application

Make sure you're in the project root directory, then run:

```bash
mvn clean install


