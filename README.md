# 📘 Requirement Analysis in Software Development

## 🔍 Introduction

This repository serves as a practical simulation of the **requirement analysis phase** in the Software Development Life Cycle (SDLC), focusing on a **Booking Management System**. It documents the process of gathering, analyzing, and modeling software requirements using industry-standard practices and tools.

The goal of this project is to demonstrate how clear, structured, and validated requirements lay the foundation for successful software development. It includes detailed documentation of functional and non-functional requirements, use cases, user stories, acceptance criteria, and supporting diagrams.

## 📌 What is Requirement Analysis?

**Requirement Analysis** is a foundational phase in the **Software Development Life Cycle (SDLC)** where the project team gathers, evaluates, and documents the needs and expectations of stakeholders for a software system. It involves understanding what the system should do (functional requirements) and how it should perform (non-functional requirements), ensuring the development team builds the right product.

This phase acts as a bridge between the client’s vision and the technical implementation. It ensures all stakeholders—developers, clients, project managers, and users—share a common understanding of the system’s goals, constraints, and expected behavior.

### 🧠 Key Objectives of Requirement Analysis:

- **Identify and define the scope** of the system.
- **Gather requirements** from all relevant stakeholders.
- **Document requirements** clearly and unambiguously.
- **Analyze and prioritize** features based on business value and feasibility.
- **Validate requirements** to ensure completeness and correctness.

### 🔍 Importance in the SDLC:

| Benefit                                    | Description                                                               |
| ------------------------------------------ | ------------------------------------------------------------------------- |
| ✅ **Clarity and Alignment**               | Ensures everyone understands what is being built and why.                 |
| 🧱 **Foundation for Design & Development** | Provides a blueprint for system architecture and functionality.           |
| 💰 **Accurate Estimation**                 | Helps in planning budgets, timelines, and resources effectively.          |
| 🔒 **Scope Control**                       | Prevents scope creep by setting clear boundaries and expectations.        |
| 📈 **Improved Quality**                    | Leads to better testing, fewer defects, and higher customer satisfaction. |

Without a thorough requirement analysis, projects risk miscommunication, rework, budget overruns, and ultimately, failure to meet user needs. Therefore, requirement analysis is not just the first step—it's the **cornerstone of successful software development**.

## 🎯 Why is Requirement Analysis Important?

Requirement Analysis is a vital phase in the Software Development Life Cycle (SDLC) because it ensures that the software is built correctly and meets user expectations. Below are key reasons why it is essential:

- **Clarity and Understanding**  
  Helps all stakeholders gain a shared understanding of what the software should do, reducing misunderstandings and ambiguity.

- **Scope Definition**  
  Clearly outlines the boundaries of the project, helping to prevent **scope creep** and maintain focus on agreed-upon goals.

- **Basis for Design and Development**  
  Acts as a blueprint for system architecture, interface design, and implementation strategies, ensuring development aligns with requirements.

- **Cost and Time Estimation**  
  Enables accurate estimation of project timelines, required resources, and overall cost by understanding the full scope and complexity.

- **Quality Assurance**  
  Ensures that the delivered product meets the specified functional and non-functional requirements, leading to improved customer satisfaction and fewer revisions.

By conducting thorough requirement analysis, development teams can minimize risk, reduce rework, and ensure a smoother path from concept to delivery.

## 🧩 Key Activities in Requirement Analysis

Requirement Analysis involves several interrelated activities that ensure the right system is built in the right way. Each step contributes to developing a complete, accurate, and actionable understanding of what the software must do.

### 1. 📥 Requirement Gathering

- Collect initial information from stakeholders through interviews, surveys, workshops, and observation.
- Review existing documentation, systems, or business processes.
- Aim to understand the goals, constraints, and expectations of end users and business owners.

### 2. ✍️ Requirement Elicitation

- Dig deeper into the gathered information to uncover detailed and hidden needs.
- Use techniques like brainstorming, focus groups, prototyping, and storyboarding.
- Facilitate collaboration among stakeholders to refine and expand requirements.

### 3. 📚 Requirement Documentation

- Document functional and non-functional requirements in a structured format (e.g., Software Requirements Specification).
- Write user stories that describe features from the end user’s perspective.
- Use use case diagrams to visually represent system interactions.

### 4. 📊 Requirement Analysis and Modeling

- Analyze the documented requirements to detect conflicts, gaps, or inconsistencies.
- Prioritize requirements based on business value, technical feasibility, and stakeholder needs.
- Create visual models such as data flow diagrams (DFD), entity-relationship diagrams (ERD), or UML diagrams to support analysis.

### 5. ✅ Requirement Validation

- Review the documented requirements with stakeholders to confirm accuracy and completeness.
- Define acceptance criteria that clearly describe when a requirement is considered "done."
- Ensure traceability between requirements and implementation to facilitate testing and change management.

Each of these activities plays a crucial role in transforming business needs into actionable development tasks that align with the project's goals and user expectations.

## 🛠️ Types of Requirements

In a booking management system like those used by Airbnb, requirements fall into two primary categories: **Functional** and **Non-functional**. Both are essential for building a feature-rich, scalable, and reliable platform.

---

### ⚙️ Functional Requirements

**Definition:**  
Functional requirements describe the specific behaviors and functions of the system—**what the system should do** to meet user needs.

**Examples for the Booking Management System:**

- **User Registration & Authentication:** Users must be able to register, log in securely, and manage their accounts.
- **Hotel Listing Management (for Managers):** Managers can create, update, and delete property listings using a dedicated portal.
- **Search Functionality:** Users can search hotels based on filters like location, date, guest count, and price using ElasticSearch.
- **Booking Flow:** Users can select a hotel, check availability, confirm a booking, and make payments via an integrated payment gateway.
- **View Bookings:** Users and hotel managers can view upcoming and past bookings via a booking history service.
- **Notification System:** Users receive real-time notifications on booking confirmation or cancellation via Kafka-powered messaging services.

---

### 🛡️ Non-functional Requirements

**Definition:**  
Non-functional requirements define **how the system performs** rather than what it does. They address quality attributes like performance, security, scalability, and reliability.

**Examples for the Booking Management System:**

- **Performance:** The system should return search results within 2 seconds even under high user load (e.g., 1000 concurrent users).
- **Scalability:** Microservices must be horizontally scalable to support peak-time traffic (e.g., during holiday booking surges).
- **Security:** All user credentials and transactions must be encrypted (SSL/TLS). Apply rate limiting and prevent SQL injection, XSS, etc.
- **Reliability:** Ensure 99.9% system uptime with automatic failover mechanisms for all major services.
- **Data Consistency:** Sync between master-slave databases should occur within milliseconds to ensure consistent booking status across services.
- **Maintainability:** Code and services must follow a modular architecture to allow independent updates and fixes.
- **Data Archival:** Older booking records must be archived in Cassandra for efficient long-term access without affecting primary databases.

---

Understanding both types of requirements ensures that the booking platform not only **functions as expected** but also **delivers a fast, secure, and seamless experience** to all users.

## 📊 Use Case Diagrams

### What is a Use Case Diagram?

A **Use Case Diagram** is a type of UML (Unified Modeling Language) diagram that visually represents the **interactions between users (actors)** and the **system (use cases)**. It helps stakeholders understand **who does what** in the system, providing a clear picture of system functionality from a user's perspective.

### 🔍 Benefits of Use Case Diagrams

- ✔️ Provides a high-level view of system functionalities
- 🧩 Helps identify system actors and their goals
- 💬 Enhances communication between technical and non-technical stakeholders
- 📋 Serves as a foundation for creating detailed user stories and test cases

---

### 👥 Actors in the Booking Management System

- **Guest/User:** Can browse listings, book hotels, and manage bookings
- **Hotel Manager:** Manages hotel listings and views bookings
- **Admin:** Manages users and monitors the system

---

### 🛠️ Key Use Cases

- Register/Login
- Search Hotels
- View Listings
- Make a Booking
- Cancel/Modify Booking
- Manage Hotel Information (Manager)
- View Booking History
- Receive Notifications
- Process Payments

---

### 🖼️ Use Case Diagram

Below is a use case diagram representing the core interactions in the Booking Management System:

![Use Case Diagram for Booking System](./alx-booking-uc.png)

> 📝 \_Diagram created using [Draw.io](https://draw.io) and exported as `alx-booking-uc.png`.

---

## ✅ Acceptance Criteria

### What is Acceptance Criteria?

**Acceptance Criteria** are predefined conditions that a feature or system must satisfy in order to be accepted by the stakeholders. They define the boundaries of a user story or requirement, clarify expectations, and serve as the basis for testing and validation.

### 🔍 Importance in Requirement Analysis

- **Clarifies Expectations:** Ensures developers and stakeholders are aligned on what a feature must deliver.
- **Improves Testability:** Provides a clear reference for writing test cases and conducting QA checks.
- **Defines Done:** Helps the team understand when a task or user story can be marked as complete.
- **Reduces Ambiguity:** Avoids misinterpretation of requirements by specifying concrete and measurable outcomes.
- **Supports User-Centered Design:** Keeps the focus on the user’s goals and success criteria.

---

### 🛒 Example: Acceptance Criteria for Checkout Feature

**Feature:** Hotel Booking Checkout

**Acceptance Criteria:**

- ✅ The user must be logged in to access the checkout page.
- ✅ The system must display selected booking details (property, dates, guests, total cost).
- ✅ Users must be able to enter or select a saved payment method.
- ✅ Payment processing must be integrated with a secure third-party provider (e.g., Stripe).
- ✅ Upon successful payment, the system should:
  - Create a booking record in the database
  - Send confirmation email and SMS to the user
  - Notify the hotel manager via the notification service
- ✅ If payment fails, the user should receive a meaningful error message and the booking should not be created.
- ✅ The booking confirmation page should be displayed within 5 seconds of successful payment.

---

Acceptance criteria ensure that software features are **testable, verifiable, and aligned** with real-world business goals. They serve as a contract between stakeholders and developers, reinforcing clarity and quality throughout the development process.
