# Database Testing

This repository contains automated tests for the database of a task management system using [Pytest](https://docs.pytest.org/en/stable/#documentation), [SQLModel](https://sqlmodel.tiangolo.com) and Python. It covers core CRUD operations, along with error handling for session failures and invalid data. The project uses fixtures for database management and ensures data integrity by isolating test cases with session rollbacks. The database tests are designed to validate data consistency and robustness under various conditions.

## 🔧 How to Run

1. Clone repository:
   ```shell
   git clone https://github.com/Eqnesto/Project.git
   ```
1. Install [Python](https://www.python.org/downloads/).
1. Open folder in [Visual Studio Code](https://code.visualstudio.com/download).
1. Install packages:
   ```shell
   pip install -r requirements.txt
   ```
3. Run tests:
   ```shell
   pytest
   ```
   
## 📄 Test Cases

1. **CRUD Operations**
   * **Create Task**: Tests adding a new task to the database.
   * **Read Task**: Tests retrieving a task by its ID.
   * **Read All Tasks**: Tests fetching all tasks from the database.
   * **Update Task Fields**: Tests updating task details.
   * **Update Timestamp**: Tests updating the `updated_at` field.
   * **Delete Task**: Tests removing a specific task.
   * **Delete All Tasks**: Tests clearing all tasks from the database.

2. **Error Handling**
   * **Read Task Not Found**: Tests behavior when task ID doesn't exist.
   * **Delete Task Not Found**: Tests deleting a non-existent task.
   * **Invalid Task Model**: Tests validation for incorrect task data.
   * **Session Failure**: Tests handling session errors.
   * **Connection Issues**: Tests database connection errors.
