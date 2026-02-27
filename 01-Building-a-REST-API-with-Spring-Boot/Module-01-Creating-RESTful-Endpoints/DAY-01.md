
#  DAY 01 – Spring and Spring Boot

##  Lesson: Spring and Spring Boot Fundamentals

---

#  What is Spring?

Spring is a comprehensive Java framework used to build enterprise applications.

It provides multiple modules such as:

- Spring MVC (Web Layer)
- Spring Data (Data Access)
- Spring Security (Authentication & Authorization)
- Spring Core (Dependency Management)

Think of Spring as a giant toolbox that contains everything required to build scalable, maintainable applications.

###  Challenge with Spring
Spring requires heavy configuration.
Developers must manually configure:
- Beans
- Dependencies
- Web server
- Data sources

This makes setup powerful but complex.

---

#  What is Spring Boot?

Spring Boot is an opinionated extension of Spring.

It simplifies application development by:

- Providing auto-configuration
- Reducing boilerplate setup
- Including embedded web servers (Tomcat)
- Offering production-ready features

Think of Spring Boot as:
"Spring with smart defaults pre-configured."

It allows developers to quickly build and run applications without extensive setup.

---

#  Spring’s Inversion of Control (IoC) Container

Spring Boot uses Spring Core’s IoC container.

## What is IoC?

Inversion of Control means:
The framework manages object creation and dependency wiring instead of the developer manually creating objects.

Instead of:

```
MyService service = new MyService();
```

Spring automatically injects dependencies at runtime.

This is commonly called **Dependency Injection (DI)**.

---

##  Why IoC is Powerful

It allows:

- Loose coupling
- Easy testing
- External configuration
- Switching environments easily

### Example:
You can configure:
- H2 database for local development
- PostgreSQL for production

Without changing application code.

Configuration is externalized.

---

#  Spring Initializr

Spring Initializr is used to bootstrap Spring Boot applications.

It acts like a dependency generator tool.

Steps:
1. Choose Project Type (Gradle / Maven)
2. Choose Language (Java)
3. Choose Spring Boot Version
4. Add Dependencies (Spring Web, etc.)
5. Generate project

It produces a ready-to-run Spring Boot application.

---

#  LAB – Spring Initializr

In this lab:

- Used Spring Initializr
- Generated a Spring Boot project
- Built the project using:

```
./gradlew build
```

###  Build Result:
BUILD SUCCESSFUL

This confirms:
- Project setup is correct
- Dependencies resolved successfully
- Application compiles and passes tests

---

#  Key Takeaways

- Spring = Powerful but configuration-heavy framework
- Spring Boot = Simplified, opinionated version of Spring
- IoC container manages dependencies
- Dependency Injection helps reduce tight coupling
- Spring Initializr bootstraps projects quickly
- Gradle build verifies successful setup

---

#  Personal Notes

- Spring Boot drastically reduces setup time.
- IoC is foundational — must understand deeply.
- Spring Initializr is essential for real-world development.
- Build success confirms correct environment configuration.

---

# ⏭ Next Topic
API Contracts & JSON
