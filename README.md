# 📝 C++ Console-Based Text Editor

A simple command-line **Text Editor in C++** using a **linked list** as the core data structure. This editor allows you to insert, delete, update, append, search, and save text—along with **Undo** and **Redo** capabilities.

---

## 🚀 Features

- Insert, delete, update, and append text
- Undo and Redo operations
- Search functionality
- Save and load text permanently from a file (`text_editor.txt`)
- Line-by-line text organization using a singly linked list

---

## 🧱 Data Structures Used

- **Singly Linked List** to store each line of text as a node
- **Stack** to implement Undo and Redo operations using snapshots of the list

---

## 📂 File Structure

text-editor/
│
├── main.cpp # Complete source code
├── text_editor.txt # Generated upon saving text permanently
└── README.md # This documentation


---

## 💻 How It Works

Each line of text is stored in a node of a linked list. The user is presented with a menu of operations. Based on the input key, the program performs the selected action and updates the text editor accordingly.

Undo/Redo works by pushing and popping snapshots of the linked list onto a stack.

---

## 📋 Menu of Operations

| Command | Action                         |
|---------|--------------------------------|
| 0       | Help (Display all commands)    |
| 1       | Insert new text                |
| 2       | Delete text by line number     |
| 3       | Update text at a specific line |
| 4       | Append text to an existing line|
| 5       | Search for specific text       |
| 6       | Display all text               |
| 7       | Save data permanently to file  |
| 8       | Undo last change               |
| 9       | Redo last undone change        |
| 10      | Exit                           |
| 11      | View saved file data           |

---

## 🛠️ How to Run

### Compile:
```bash
g++ main.cpp -o texteditor


Run:
bash
./texteditor

Example Use Cases
Create and edit multiline notes or documents

Practice and understand linked lists, file I/O, and stack-based operations

Command-line based editing simulation for educational purposes


Notes
Make sure to use getline() twice after cin >> when mixing cin and getline to avoid input buffer issues.

The default number of text lines is not restricted — works dynamically.
