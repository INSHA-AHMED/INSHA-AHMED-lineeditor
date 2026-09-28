# 📝 Simple Line Editor in C

A command-line line editor built in C for creating, viewing, modifying, saving, and searching a document one line at a time.

## 👥 Team Members

| Name | Roll Number |
|---|---|
| Insha Ahmed | R25EJ043 |
| J Karthik Raj | R25EJ045 |
| Krithik D Shetty | R25EJ056 |

## 📌 About the Project

This project implements a simple command-line line editor in C. It stores document lines using a dynamic array of strings and provides commands for inserting, deleting, displaying, saving, loading, searching, and counting document content.

The project applies:

- Data structures
- Arrays and pointers
- Strings
- Functions
- Dynamic memory allocation
- File handling
- Command-line input handling

## ✨ Features

### Core Features

- **Insert** — insert text at a specified line number.
- **Delete** — delete an existing line.
- **Display** — display all lines with their line numbers.

### Additional Features

- **Save** — save the current document to a text file.
- **Load** — load a text file into the editor.
- **Search** — search for a word or phrase and show matching line numbers.
- **Count** — display the number of lines and words.
- **Help** — display command descriptions and usage examples.
- **Quit/Exit** — close the editor.

## 🗂️ Project Structure

```text
lineeditor/
├── README.md
├── .gitignore
└── src/
    ├── main.c
    └── Help.txt
```

## 🛠️ Compile and Run

### Clone the repository

```bash
git clone https://github.com/INSHA-AHMED/lineeditor.git
cd lineeditor
```

### Compile with GCC

```bash
gcc -Wall -Wextra -std=c11 src/main.c -o editor
```

### Run

**Windows:**

```text
.\editor.exe
```

**Linux/macOS:**

```bash
./editor
```

### Optional: Load a file at startup

```bash
./editor document.txt
```

On Windows, use:

```text
.\editor.exe document.txt
```

## ⌨️ Commands

```text
insert <line> <text>
delete <line>
display
save <filename>
load <filename>
search <word or phrase>
count
help
quit
```

See [`src/Help.txt`](src/Help.txt) for command descriptions and usage examples.

## 📚 Data Structure

The editor uses a **dynamic array of strings**. Each document line is stored as a dynamically allocated string, while the array of line pointers grows using `realloc()` when additional capacity is required.
