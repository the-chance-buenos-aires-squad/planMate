# PlanMate

PlanMate is a collaborative project management system designed to help teams organize their work, track tasks, and maintain full visibility over progress and changes across projects.

It was built to solve the problem of fragmented task tracking in team environments by providing a structured system for managing projects, responsibilities, and workflow states in a single CLI-based application.

The system emphasizes clarity, accountability, and traceability through role-based access control and a full audit logging system.

---

## Key Features

### 📌 Task Management

* Create, update, and track tasks across different workflow states
* Support for task lifecycle (TODO → In Progress → Done)
* Organize tasks under specific projects for better structure

### 📁 Project Management

* Create and manage multiple projects
* Assign and group tasks under projects
* Track overall project progress

### 👤 Role-Based Access Control

* Admin and User roles
* Controlled access to system operations based on permissions
* Secure management of sensitive actions

### 🧾 Audit Logging System

* Track all changes made to tasks and projects
* Record who made changes, when, and what was changed
* Maintain full history for accountability and transparency

### 📊 CLI Swimlane View

* Visual representation of tasks by status
* Quick overview of project progress directly in terminal

### 💾 Flexible Data Storage

* MongoDB as primary database
* CSV-based legacy support
* Repository abstraction enabling easy switching between data sources

---

## Architecture

PlanMate follows Clean Architecture principles to ensure separation of concerns and long-term maintainability.

### Layers:

* **Domain Layer**
  Contains business logic, entities, and use cases. Independent from frameworks and external tools.

* **Data Layer**
  Handles data persistence using MongoDB and CSV implementations. Uses repository pattern and mappers.

* **Presentation Layer**
  CLI interface responsible for user interaction and command handling.

---

## Technical Highlights

* Kotlin-based CLI application
* Clean Architecture design
* SOLID principles applied across the system
* Dependency Inversion for flexible data storage
* Koin for dependency injection
* Test-Driven Development (TDD)
* JUnit 5, MockK, and Truth for testing

---

## What This Project Demonstrates

This project demonstrates the ability to:

* Design scalable and maintainable software systems
* Apply Clean Architecture in real-world applications
* Build role-based systems with proper access control
* Implement audit logging for full system traceability
* Manage data migration between storage systems
* Write testable and modular Kotlin code
* Collaborate effectively using Git-based workflows

---

## Getting Started

### Requirements

* Java 17+
* Gradle 8+
* MongoDB (optional depending on configuration)

### Setup

```bash id="1a2b3c"
git clone https://github.com/the-chance-buenos-aires-squad/planMate.git
cd planMate
```

### Build

```bash id="4d5e6f"
./gradlew build
```

### Run

```bash id="7g8h9i"
./gradlew run
```

### Tests

```bash id="0j1k2l"
./gradlew test
```

---

### 📝 License

This project is licensed under the Chance License.
