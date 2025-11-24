# Project Statement: Gym Membership Management Application

## 1. Purpose and Scope

The Gym Membership Management Application is designed to provide a simple, localized tool for managing member records.

**Primary Objectives:**
* Streamline the process of registering, viewing, and updating gym membership information.
* Provide a foundational command-line interface for practical data management demonstration.

The scope of this application is limited to in-memory data management within a single runtime session.

## 2. Data Handling and Persistence Policy

### 2.1. Data Type

The application handles standard member attributes:
* Member ID (System-assigned, unique integer)
* Name (String)
* Age (Integer)
* Membership Type (String, e.g., Monthly, Yearly)

### 2.2. Persistence

**CURRENT STATUS:** This application currently operates purely with **in-memory storage**.

* All member data is stored in the `self.members` dictionary within the `GymMembershipApp` instance.
* When the program is terminated (Option 6: Exit or closing the console), **all unsaved data is lost.**
* No external database or file system is currently utilized for persistent storage.

## 3. Future Development Commitment

We are committed to enhancing the utility and robustness of this application.

**Future Considerations Include:**
1.  **Data Persistence:** Implementing functionality to save and load member data to an external file (e.g., JSON or CSV) to prevent data loss upon exit.
2.  **Input Validation:** Enhancing robustness by adding strict checks for input types (e.g., ensuring age is an integer and membership type is a valid option).
3.  **Reporting:** Adding features to generate simple reports (e.g., count of members per membership type).

---

*This statement was last updated on 2025-11-24.*
