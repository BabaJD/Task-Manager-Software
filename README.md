# Task Manager Software

## Description

This Python-based Task Manager application is a command-line tool for managing your to-do list. It offers basic CRUD (Create, Read, Update, Delete) operations for tasks, along with persistent storage using a JSON file.

Key features include:

* **Task Creation:** Add new tasks with a title and description.
* **Task Listing:** View all tasks in your list.
* **Task Updating:** Modify the title or description of existing tasks.
* **Task Deletion:** Remove tasks from your list.
* **Data Persistence:** Your tasks are saved in a JSON file so they persist between sessions.

This project was valuable for understanding:

* **Object-Oriented Programming (OOP):** It uses classes (`Task`, `TaskManager`, `DataAccessLayer`, `FileStorage`) to structure the code and encapsulate different functionalities.
* **Data Persistence:** It demonstrates how to save and load data using a simple JSON file, providing a basic introduction to data storage.
* **User Interface:** It includes a text-based menu for user interaction, showcasing how to handle user input and provide feedback.
* **Software Design:** It illustrates concepts like separation of concerns (DAL, storage) and modularity, making the code more organized and maintainable.
* **Code Formatting and Linting:** The project includes tools like Black and Flake8 to enforce code style and quality, which are important best practices in Python development.


## Installation

1. **Clone the Repository:** (Assuming you have the code hosted on a platform like GitHub)
   ```bash
   git clone <repository_url>
   ```
2. **Create a Virtual Environment:**
   ```bash
   python -m venv env
   ```
3. **Activate the virtual environment:**
   ```bash
   # For Linux/macOS
   source env/bin/activate
   # For Windows
   .\env\Scripts\activate
   ```
4. **Install Dependencies:**
   ```bash
   pip install black==24.4.2 click==8.1.7 colorama==0.4.6 distlib==0.3.8 filelock==3.14.0 flake8==7.0.0 mccabe==0.7.0 mypy-extensions==1.0.0 packaging==24.0 pathspec==0.12.1 platformdirs==4.2.2 pycodestyle==2.11.1 pyflakes==3.2.0 virtualenv==20.26.2
   ```
   

## Usage

1. **Run the script:** 
   ```bash
   python main.py
   ```

2. **Interact with the Menu:**
    * **Create Task:**
        * Choose option `1` from the menu.
        * Enter the task title and description when prompted.
    * **Read Tasks:**
        * Choose option `2` to display a numbered list of all your tasks.
    * **Update Task:**
        * Choose option `3`.
        * Enter the number of the task you want to update.
        * Enter the new title and description.
    * **Delete Task:**
        * Choose option `4`.
        * Enter the number of the task you want to delete.
    * **Exit:**
        * Choose option `5` to quit the application.


## Project Structure

* `main.py`: The main script that runs the Task Manager.
* `task.py`: Defines the `Task` class representing a task item.
* `data_access_layer.py`: Contains the `DataAccessLayer` class for interacting with the storage.
* `file_storage.py`:  Implements the `FileStorage` class for saving and loading tasks to/from a JSON file.
* `tasks.json`: The file where task data is stored.

## Credits

* **Author:** Babajide Abraham Alamu
