# Sanghamitra-Malakar-25BAI10731
# 🏋️ Gym Membership Management Application

This is a simple command-line Python application for managing gym members. It uses a class-based structure (`GymMembershipApp`) to handle basic CRUD (Create, Read, Update, Delete) operations on member records.

## ✨ Features

* **Add Member:** Register a new member with a name, age, and initial membership type. Automatically assigns a unique member ID.
* **View Members:** Display a list of all currently registered members and their details.
* **Search Member:** Find a specific member by their unique ID.
* **Update Membership:** Change the membership type (e.g., Monthly to Yearly) for an existing member.
* **Delete Member:** Remove a member's record from the system using their ID.

## 🚀 How to Run

### Prerequisites

You need to have **Python 3** installed on your system.

### Steps

1.  **Save the Code:** Save the provided Python code into a file named, for example, `gym_app.py`.
2.  **Run from Terminal:** Open your terminal or command prompt, navigate to the directory where you saved the file, and run the following command:

    ```bash
    python gym_app.py
    ```

3.  **Use the Menu:** The application will start and present a menu. Enter the number corresponding to the action you wish to perform (1 through 6).

## 💡 How It Works

The application is built around the `GymMembershipApp` class, which manages member data using a Python dictionary:

* **Data Storage:** Member data is stored in the `self.members` dictionary, where the **key** is the unique integer `member_id`, and the **value** is another dictionary containing the member's details (`name`, `age`, `membership`).
* **ID Management:** The `self.member_id` instance variable automatically increments to ensure every new member receives a unique ID.
* **Main Loop:** The `main()` function provides the interactive command-line menu, continuously prompting the user for an action until the "Exit" option is chosen.

## 🛠️ Implementation Details (For Developers)

| Method | Description | Data Structure Operation |
| :--- | :--- | :--- |
| `__init__` | Initializes the member storage dictionary and the starting member ID. | Initialization |
| `add_member` | Adds a new key-value pair to `self.members`. | Dictionary **Create** |
| `view_members` | Iterates over all key-value pairs in `self.members`. | Dictionary **Read (All)** |
| `search_member` | Uses `self.members.get(member_id)` for quick lookup. | Dictionary **Read (Specific)** |
| `update_membership`| Modifies the value associated with an existing member ID key. | Dictionary **Update** |
| `delete_member` | Uses `self.members.pop(member_id)` to remove an entry. | Dictionary **Delete** |

---

## 📝 Example Session

1.  **Run the app:**
    ```bash
    python gym_app.py
    ```
2.  **Add Member (Choice 1):** Enter details.
3.  **View Members (Choice 2):** See the newly added member's record.
4.  **Search Member (Choice 3):** Enter the ID (e.g., `1`) to confirm details.
5.  **Exit (Choice 6):** Terminate the application.
