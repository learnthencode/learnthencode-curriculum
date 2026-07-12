# The Command Line

## Overview

Most people interact with their computers using a graphical interface.

They click icons, open folders, drag files, and launch applications using a mouse or touchpad.

Professional software engineers also use these graphical interfaces, but they frequently rely on another powerful way of interacting with computers: the **command line**.

The command line allows developers to communicate directly with the operating system by typing commands.

Although it may seem unfamiliar at first, it is one of the most important tools in software engineering. Many development tools, programming languages, cloud platforms, and automation systems are designed to work from the command line.

Throughout this bootcamp, you will use the command line almost every day.

In this lesson, you will learn what the command line is, why software engineers use it, and how to navigate your computer using terminal commands.

The goal is simple:

> **Understand the command line first, then use it to work more efficiently.**

---

## Learning Objectives

By the end of this lesson, you should be able to:

- Explain the difference between a graphical user interface (GUI) and a command-line interface (CLI).
- Explain what a terminal is.
- Explain what a shell is.
- Understand how commands are processed.
- Open the terminal on Windows, macOS, and Linux.
- Understand files, folders, and the file system.
- Navigate directories using terminal commands.
- Create, move, rename, copy, and delete files and folders.
- Use common terminal shortcuts.
- Organize projects using the command line.

---

## Why This Matters

Many beginners wonder why software engineers still use the command line when modern operating systems provide beautiful graphical interfaces.

The answer is simple.

The command line is often:

- Faster.
- More precise.
- Easier to automate.
- Better suited for development tools.
- Available on almost every computer and server.

Many professional tools—including Git, Node.js, Python, Docker, Linux servers, and cloud platforms—are primarily designed to be used from the command line.

Learning the command line is not about replacing graphical applications.

It is about gaining another powerful way to communicate with your computer.

---

# Sub-lessons

## Graphical User Interface (GUI) vs Command-Line Interface (CLI)

There are two common ways to interact with a computer.

### Graphical User Interface (GUI)

A **Graphical User Interface (GUI)** allows users to interact with computers using visual elements such as:

- Windows
- Icons
- Menus
- Buttons
- Mouse clicks
- Touch gestures

Examples include:

- Windows Desktop
- macOS Finder
- Ubuntu Desktop
- File Explorer

Most people use GUIs every day.

For example, when you:

- Open Google Chrome
- Create a folder
- Move a file
- Delete a document

you are using a graphical interface.

---

### Command-Line Interface (CLI)

A **Command-Line Interface (CLI)** allows users to communicate with the operating system by typing commands instead of clicking buttons.

Instead of this:

```text
Right Click
      ↓
New Folder
```

you type a command such as:

```bash
mkdir projects
```

Both methods achieve the same result.

The difference is simply how you communicate with the computer.

---

### Comparing GUI and CLI

| GUI | CLI |
|------|------|
| Uses windows and icons | Uses text commands |
| Easy for beginners | Requires learning commands |
| Great for everyday tasks | Excellent for automation and development |
| Mouse-driven | Keyboard-driven |
| Slower for repetitive work | Faster for repetitive work |

Neither interface is better.

Professional software engineers use **both** depending on the task.

---

## What Is a Terminal?

A **terminal** is the application that allows you to use the command line.

Think of the terminal as a conversation window between you and your computer.

You type commands.

The operating system performs the requested task.

The terminal displays the result.

The interaction looks like this:

```text
Developer
     │
     ▼
 Terminal
     │
     ▼
 Shell
     │
     ▼
Operating System
     │
     ▼
 Computer Hardware
```

Different operating systems provide different terminal applications.

| Operating System | Default Terminal |
|------------------|------------------|
| Windows | Windows Terminal or PowerShell |
| macOS | Terminal |
| Linux | Terminal |

Although they look different, they all serve the same purpose.

---

## What Is a Shell?

Many beginners think the terminal and the shell are the same thing.

They are closely related but not identical.

The **terminal** is the application you open.

The **shell** is the program running inside the terminal that interprets your commands.

When you type:

```text
mkdir projects
```

the shell reads your command, understands what it means, asks the operating system to create the folder, and then displays the result.

Think of the shell as an interpreter between you and your computer.

Some common shells include:

| Shell | Common Operating Systems |
|--------|--------------------------|
| PowerShell | Windows |
| Bash | Linux, macOS |
| Zsh | macOS |
| Fish | Linux, macOS |

Throughout this bootcamp, you will primarily use:

- **PowerShell** on Windows.
- **Terminal (Zsh or Bash)** on macOS.
- **Bash** on Linux.

---

## Opening the Terminal

Before you can use the command line, you need to open your terminal application.

### Windows

1. Open the **Start Menu**.
2. Search for **Windows Terminal**.
3. Open the application.

If Windows Terminal is unavailable, open **PowerShell** instead.

---

### macOS

1. Open **Spotlight Search** (`⌘ + Space`).
2. Search for **Terminal**.
3. Press **Enter**.

---

### Linux

Most Linux distributions include a Terminal application.

Open your Applications menu and search for **Terminal**.

---

## Understanding the Command Prompt

After opening the terminal, you will see something similar to this.

### Windows

```powershell
PS C:\Users\Yahya>
```

### macOS

```bash
yahya@MacBook ~ %
```

### Linux

```bash
yahya@ubuntu:~$
```

This is called the **command prompt**.

The command prompt indicates that the shell is ready to receive your commands.

Think of it as your computer saying:

> "I'm ready. What would you like me to do?"

---

## Running Your First Commands

Let's begin with a few safe commands.

### Display a Message

| Windows (PowerShell) | macOS / Linux | Purpose |
|-----------------------|---------------|---------|
| `echo Hello, LearnThenCode!` | `echo Hello, LearnThenCode!` | Display text on the terminal |

Expected output:

```text
Hello, LearnThenCode!
```

---

### Clear the Terminal

After running several commands, your screen may become cluttered.

Use the following commands to clear it.

| Windows (PowerShell) | macOS / Linux | Purpose |
|-----------------------|---------------|---------|
| `cls` | `clear` | Clears the terminal screen |

---

### Exit the Terminal

When you finish using the terminal, you can close it by typing:

| Windows | macOS | Linux | Purpose |
|----------|--------|--------|---------|
| `exit` | `exit` | `exit` | Closes the terminal session |

Congratulations!

You have successfully interacted with your computer using the command line.

In the next section, you will learn how software engineers navigate the file system and organize projects using terminal commands.

## Understanding the File System

Before you can navigate your computer using the command line, you need to understand how files are organized.

Every operating system stores information using a **file system**.

A file system is a way of organizing files and folders so that they can be stored, located, and managed efficiently.

Think of it like a filing cabinet.

```text
Filing Cabinet
│
├── Drawer
│   ├── Folder
│   │   ├── Document
│   │   └── Document
│   └── Folder
│
└── Drawer
```

Your computer works in a similar way.

```text
Computer
│
├── Users
│   └── Yahya
│       ├── Desktop
│       ├── Documents
│       ├── Downloads
│       ├── Pictures
│       └── Music
```

Folders can contain other folders.

Folders can also contain files.

---

## Files and Directories

You will frequently hear two terms:

- **File**
- **Directory**

A **file** stores information.

Examples include:

- `notes.md`
- `index.html`
- `script.js`
- `photo.png`

A **directory** (also called a **folder**) is a container used to organize files and other directories.

For example:

```text
learnthencode
│
├── notes.md
├── projects
│   ├── website
│   └── calculator
└── assignments
```

In this example:

- `learnthencode` is a directory.
- `projects` is a directory.
- `website` is a directory.
- `notes.md` is a file.

---

## Understanding Paths

A **path** tells the computer where a file or directory is located.

Imagine giving someone directions to your house.

Instead of saying:

> "It's somewhere in Mombasa."

you provide the complete address.

Paths work in the same way.

Example:

```text
Users
└── Yahya
    └── Documents
        └── learnthencode
            └── notes.md
```

The path to the file is:

```text
Users/Yahya/Documents/learnthencode/notes.md
```

---

## Absolute Paths

An **absolute path** starts from the beginning of the file system.

Examples:

### Windows

```text
C:\Users\Yahya\Documents\learnthencode
```

### macOS

```text
/Users/yahya/Documents/learnthencode
```

### Linux

```text
/home/yahya/Documents/learnthencode
```

An absolute path always points to the same location.

---

## Relative Paths

A **relative path** starts from your current location.

Suppose you are already inside:

```text
Documents
```

and it contains:

```text
Documents
└── learnthencode
```

Instead of typing the full path, you can simply type:

```text
learnthencode
```

Relative paths are shorter and are used frequently by software engineers.

---

## Current Working Directory

The **Current Working Directory (CWD)** is the directory you are currently working in.

Think of it as your current location on your computer.

Every command you run operates relative to this location unless you specify another path.

---

## Displaying the Current Directory

To display your current working directory, use:

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `pwd` | `pwd` | Shows your current working directory |

Example:

```powershell
PS C:\Users\Yahya\Documents>
```

Output:

```text
C:\Users\Yahya\Documents
```

On Linux or macOS:

```bash
pwd
```

Output:

```text
/home/yahya/Documents
```

The `pwd` command stands for **Print Working Directory**.

---

## Listing Files and Directories

To see what is inside your current directory, use:

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `dir` or `ls` | `ls` | Lists files and directories |

Example:

```bash
ls
```

Output:

```text
Desktop
Documents
Downloads
Pictures
Music
```

Windows PowerShell also supports `ls` as an alias for `dir`.

Throughout this course, you may use either command on Windows.

---

## Changing Directories

To move into another directory, use the `cd` command.

`cd` stands for **Change Directory**.

Suppose your current directory contains:

```text
Documents
│
└── learnthencode
```

To enter the folder:

| Windows | macOS / Linux | Purpose |
|----------|---------------|---------|
| `cd learnthencode` | `cd learnthencode` | Moves into a directory |

After running the command:

```text
Documents
    ↓
learnthencode
```

Your current working directory changes.

---

## Moving Up One Directory

Sometimes you need to move back.

Use:

| Windows | macOS / Linux | Purpose |
|----------|---------------|---------|
| `cd ..` | `cd ..` | Moves to the parent directory |

Example:

```text
Documents
└── learnthencode
```

If you are inside `learnthencode` and execute:

```bash
cd ..
```

you return to:

```text
Documents
```

---

## Returning to Your Home Directory

Your **home directory** is your personal workspace.

To return there quickly:

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `cd ~` | `cd ~` | Go to your home directory |

This command works regardless of your current location.

---

## Creating Directories

To create a new directory:

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `mkdir projects` | `mkdir projects` | Creates a new directory |

Example:

Before:

```text
Documents
```

Run:

```bash
mkdir projects
```

After:

```text
Documents
└── projects
```

---

## Creating Files

Different operating systems use different commands.

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `New-Item notes.md` | `touch notes.md` | Creates a new file |

After creating the file:

```text
projects
└── notes.md
```

Later in this bootcamp, Visual Studio Code will also allow you to create files graphically.

---

## Viewing Command History

The terminal remembers commands you have previously executed.

Instead of typing the same command repeatedly, press:

| Key | Purpose |
|-----|---------|
| ↑ | Previous command |
| ↓ | Next command |

This simple shortcut saves a significant amount of time.

---

## Using Tab Completion

Typing long file names can become tedious.

Instead of typing the entire name, type the first few letters and press:

```text
Tab
```

The shell will attempt to complete the file or directory name automatically.

Professional developers use this feature constantly.

It reduces typing and helps avoid spelling mistakes.

## Copying Files

Sometimes you need to create a copy of an existing file.

Instead of creating a new file from scratch, you can copy it.

### Copy a File

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `Copy-Item notes.md notes-copy.md` | `cp notes.md notes-copy.md` | Copies a file |

Example:

Before:

```text
projects
└── notes.md
```

Run the appropriate command.

After:

```text
projects
├── notes.md
└── notes-copy.md
```

Copying files allows you to create backups or duplicate existing work without affecting the original file.

---

## Moving and Renaming Files

The same command can often be used to move files to another directory or rename them.

### Rename a File

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `Rename-Item notes.md lesson-notes.md` | `mv notes.md lesson-notes.md` | Renames a file |

Example:

Before:

```text
notes.md
```

After:

```text
lesson-notes.md
```

---

### Move a File

Suppose you have the following structure:

```text
Documents
├── notes.md
└── projects
```

To move `notes.md` into the `projects` folder:

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `Move-Item notes.md projects` | `mv notes.md projects` | Moves a file |

Result:

```text
Documents
└── projects
    └── notes.md
```

Moving files helps keep projects organized as they grow.

---

## Deleting Files

Sometimes files are no longer needed.

Be careful when deleting files because they may not be easy to recover.

### Delete a File

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `Remove-Item notes.md` | `rm notes.md` | Deletes a file |

Example:

Before:

```text
projects
├── notes.md
└── lesson.md
```

After deleting `notes.md`:

```text
projects
└── lesson.md
```

Always double-check the file name before deleting it.

---

## Deleting Empty Directories

If a directory is empty, it can be removed.

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `Remove-Item empty-folder` | `rmdir empty-folder` | Removes an empty directory |

Example:

Before:

```text
projects
└── old-project
```

After:

```text
projects
```

Some operating systems require additional options when deleting directories that contain files. We will learn those commands later in the bootcamp.

---

## Terminal Shortcuts

Professional software engineers use keyboard shortcuts constantly.

Learning these shortcuts will make you much faster.

| Shortcut | Purpose |
|----------|---------|
| ↑ | Previous command |
| ↓ | Next command |
| Tab | Auto-complete file and directory names |
| `Ctrl + C` | Cancel the currently running command |
| `Ctrl + L` | Clear the terminal screen (Linux/macOS) |
| `cls` | Clear the terminal screen (PowerShell) |
| `history` *(Linux/macOS)* | Display previously executed commands |

Don't worry if you don't remember all of these immediately.

With regular practice, they will become second nature.

---

## Organizing Your Projects

Professional software engineers keep their projects organized.

Instead of saving files in random locations, they create a dedicated workspace.

For this bootcamp, create the following directory structure inside your **Documents** folder.

```text
Documents
└── learnthencode
    ├── developer-foundations
    ├── web-development
    ├── programming-with-javascript
    ├── frontend-engineering
    ├── backend-engineering
    ├── databases
    ├── full-stack-engineering
    └── playground
```

Each folder has a purpose.

| Folder | Purpose |
|---------|---------|
| developer-foundations | Exercises from this course |
| web-development | HTML and CSS projects |
| programming-with-javascript | JavaScript exercises and projects |
| frontend-engineering | React and frontend applications |
| backend-engineering | Backend projects and APIs |
| databases | Database exercises |
| full-stack-engineering | Full-stack applications |
| playground | Experimenting with ideas and testing code |

Keeping your work organized makes projects easier to locate and maintain.

---

# Practical Activity / Lab

## Build Your First Developer Workspace

Using your terminal, complete the following tasks.

1. Open your terminal.
2. Navigate to your **Documents** folder.
3. Create a directory named `learnthencode`.
4. Navigate into the `learnthencode` directory.
5. Create the following directories:

- developer-foundations
- web-development
- programming-with-javascript
- frontend-engineering
- backend-engineering
- databases
- full-stack-engineering
- playground

6. Navigate into the `developer-foundations` directory.
7. Create a file named `notes.md`.
8. Create a second file named `commands.md`.
9. Rename `commands.md` to `terminal-commands.md`.
10. Copy `notes.md` to `notes-copy.md`.
11. Delete `notes-copy.md`.
12. Return to your home directory.

After completing the activity, your workspace should resemble the following:

```text
Documents
└── learnthencode
    ├── developer-foundations
    │   ├── notes.md
    │   └── terminal-commands.md
    ├── web-development
    ├── programming-with-javascript
    ├── frontend-engineering
    ├── backend-engineering
    ├── databases
    ├── full-stack-engineering
    └── playground
```

If you encounter any errors, read the error message carefully before trying again.

Learning to troubleshoot is an important part of becoming a software engineer.

---

# Key Takeaways

- The file system organizes files and directories on your computer.
- The terminal allows you to navigate and manage the file system efficiently.
- Developers use commands to create, copy, move, rename, and delete files and directories.
- Understanding paths and the current working directory makes navigation easier.
- Keyboard shortcuts improve productivity.
- Keeping projects organized is an essential professional habit.

---

# Summary

In this lesson, you learned:

- The difference between a GUI and a CLI.
- What a terminal and a shell are.
- How commands are processed.
- How to open and use the terminal.
- How to navigate the file system.
- How to create, copy, move, rename, and delete files and directories.
- How to organize your development workspace.
- How professional developers use the command line every day.

Remember:

> **The command line is more than a tool—it is one of the primary ways software engineers communicate with their computers. Mastering it will make you a faster, more confident, and more capable developer.**

---

# Before You Continue

Before moving to the next lesson, make sure you can confidently:

- [ ] Explain the difference between a GUI and a CLI.
- [ ] Explain the difference between a terminal and a shell.
- [ ] Open the terminal on your operating system.
- [ ] Navigate between directories.
- [ ] Display your current working directory.
- [ ] List files and directories.
- [ ] Create directories and files.
- [ ] Copy, move, rename, and delete files.
- [ ] Organize projects using the command line.

If you are unsure about any of the above, review this lesson before continuing.

---

# What's Next?

Now that you can confidently use the command line, the next lesson introduces:

**Version Control**

You will learn why professional software engineers use version control systems to track changes, collaborate with others, and manage software projects with confidence.