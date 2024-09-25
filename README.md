# 🗂️ File and Folder Management System

### ⏰ Time Required: 48 - 72 hours

---

## 👋 Introduction

Welcome coder 👩‍💻👨‍💻

For this challenge, you need to develop a backend **File and Folder Management System**. The system should allow users to create, organize, and manage folders and files, where folders can contain other folders or files, and files cannot contain any other items.

We will assess the following:

1. Data modeling and relationships
2. API design and best practices
3. Error handling and validation
4. Performance and efficiency
5. Innovation in implementation

---

## ⚔️ Challenge

![Important!](https://img.shields.io/badge/Important-Read%20the%20challenge%20thoroughly%20before%20proceeding-red?style=for-the-badge&logo=react&link=# "Important")

You are tasked with developing a backend **File and Folder Management System** that allows users to create and manage folders and files. For every user there will be a **root folder** that contains all his/her folders and files. Below is a detailed breakdown of the mandatory features and functionality you need to implement.

---

### 🗃️ Folder Management (Mandatory)

- Users should be able to create folders that can contain files or other folders.
- Folders can be nested within other folders (hierarchical structure).
- **Folder Operations**:
  - Create a new folder inside an existing folder.
  - Rename a folder.
  - Delete a folder (and all its sub-folders and files recursively).
  - Move a folder to another folder.

---

### 📄 File Management (Mandatory)

- Users should be able to create files within folders.
- Files **cannot** contain any other items (i.e., no nesting under files).
- **File Operations**:
  - Create a new file inside a folder.
  - Rename a file.
  - Delete a file.
  - Move a file to another folder.

---

### 🧭 Folder Navigation and Listing (Mandatory)

- Provide an API to list all contents of a folder, including sub-folders and files.

  
---

### 🧑‍💻 API Endpoints (Mandatory)

Create the following API endpoints for managing files and folders:

- **Folder Operations**:
  - Create a new folder (inside another folder or in the root folder).
  - Rename an existing folder.
  - Delete a folder and all its contents (recursive deletion). User cannot delete his root folder.
  - Move a folder to another folder.

- **File Operations**:
  - Create a new file inside a folder.
  - Rename an existing file.
  - Delete a file.
  - Move a file to another folder.

- **Folder Information**:
  - List all contents (files and folders) of a specified folder.

---

### 🧰 Tools and Guidelines

- **Backend Framework**: Use a framework like Django, Flask, FastAPI, or Node.js.
- **Database**: Use a relational database like PostgreSQL, MySQL, or SQLite for storing the folder and file structure.
  
#### Folder and File Structure:
- Each entry in the system will have:
  - `id`: Unique identifier.
  - `name`: The name of the folder or file.
  - `type`: Should be `folder` or `file`.
  - `parent_id`: The ID of the parent folder (or null if it’s a root folder).
  
#### Key Restrictions:
- Only folders can act as parents, meaning files **cannot** be parents.
- Recursive deletion must be implemented for folders (i.e., deleting a folder deletes all sub-items).

---

## 🏗️ Good to Have Features 
- 🔍 Search - Implement a search functionality to find files or folders by name within the system. 

## 📜 Guidelines 
- Ensure the code is clean and well-organized. 
- Commit your code as a public repository on GitHub and share the link with us.
- Include a detailed `README.md` that explains:   - Your choice of framework and database.
- The architecture of your solution.
- Any improvements or additional features you would implement if you had more time.