# Development Environment Setup

## Overview

Before writing your first line of code, you need to prepare your computer for software development.

Professional software engineers use a collection of tools that allow them to write, test, debug, and manage software efficiently. Together, these tools form what is known as a **development environment**.

A properly configured development environment helps you work more efficiently, reduces technical problems, and provides a consistent experience throughout your learning journey.

In this lesson, you will learn what a development environment is, why it is important, and how to safely prepare your computer for software development regardless of whether you use Windows, macOS, or Linux.

The goal is simple:

> **Understand your tools first, then use them with confidence.**

---

## Learning Objectives

By the end of this lesson, you should be able to:

- Explain what a development environment is.
- Understand the role of an operating system in software development.
- Identify the tools required to begin software development.
- Download software safely from official sources.
- Explain what package managers are and why developers use them.
- Install Visual Studio Code on your operating system.
- Open and use your computer's terminal.
- Create your first development workspace.
- Verify that your development environment is ready for the lessons ahead.
- Troubleshoot common installation problems.

---

## Why This Matters

Many beginners believe software development begins by opening a code editor and writing code.

Professional software engineers know that successful development starts much earlier.

Before any code is written, engineers prepare an environment that allows them to build, test, and maintain software efficiently.

Imagine trying to build a house without first gathering the necessary tools.

Even if you know how to build, your progress will be slow and frustrating.

Software development works the same way.

A properly prepared development environment allows you to focus on learning instead of constantly fighting technical problems.

The time you invest now will save you countless hours throughout this course.

---

# Sub-lessons

## What Is a Development Environment?

A **development environment** is the collection of hardware, software, and tools that developers use to build software.

Think of it as your digital workspace.

Just as a carpenter needs a workshop equipped with tools, a software engineer needs a computer prepared for software development.

A typical development environment includes:

- An operating system
- A code editor
- A terminal
- Programming languages
- Development tools
- Version control software
- Web browsers
- Internet access

Together, these tools make it possible to write, test, debug, and manage software.

A simplified view looks like this:

```text
Computer
      ↓
Operating System
      ↓
Development Tools
      ↓
Your Software Projects
```

Throughout this course, you will gradually build your development environment as new tools become necessary.

This allows you to understand each tool before using it.

---

## Understanding Operating Systems

An **operating system (OS)** is the software that manages your computer's hardware and allows applications to run.

Without an operating system, your computer would not know how to communicate with its hardware or execute programs.

Some of the most common operating systems are:

- Windows
- macOS
- Linux

Although these operating systems look different, they all perform similar responsibilities, including:

- Managing files and folders.
- Running applications.
- Managing memory.
- Communicating with hardware.
- Providing security.

Throughout this course, we will provide installation instructions for all three operating systems whenever necessary.

Regardless of which operating system you use, the software engineering concepts you learn remain the same.

---

## Choosing Your Operating System

Every operating system has strengths and weaknesses.

There is no single "best" operating system for software development.

Instead, professional developers choose the operating system that best fits their needs.

If you already own a computer, continue using its operating system throughout this course.

You do **not** need to purchase another computer.

Throughout LearnThenCode, we support:

- Windows
- macOS
- Linux

Whenever installation steps differ, we will provide separate instructions for each operating system.

---

## Downloading Software Safely

Software developers install many tools throughout their careers.

It is important to download software safely.

Whenever possible, download software only from its official website.

For example:

- Visual Studio Code → https://code.visualstudio.com
- Git → https://git-scm.com
- Python → https://python.org

Avoid downloading software from unfamiliar websites because unofficial downloads may contain outdated or malicious software.

A good habit is to verify that the website address matches the official website before downloading anything.

Developing safe habits protects both your computer and your projects.

---

## Understanding Software Installation

Installing software means copying an application's files onto your computer and preparing it for use.

Different operating systems install software differently.

Some applications use graphical installers.

Others can be installed directly from the terminal using package managers.

During this course, you will encounter both approaches.

Whenever we install a new tool, we will explain:

- What the tool is.
- Why developers use it.
- How to install it.
- How to verify the installation.
- Common problems.
- How to troubleshoot those problems.

Our goal is not simply to help you install software.

Our goal is to help you understand the installation process.

---

## Understanding Package Managers

As developers, we frequently install, update, and remove software.

Doing this manually every time would be slow and repetitive.

A **package manager** is a tool that automates software installation and management.

Think of it as an app store for developers.

Different operating systems use different package managers.

Examples include:

| Operating System | Common Package Manager |
| ---------------- | ---------------------- |
| Windows | Winget |
| macOS | Homebrew |
| Ubuntu Linux | APT |
| Fedora Linux | DNF |

You do not need to learn every package manager.

Instead, you only need to become familiar with the one used by your operating system.

As you progress through this course, you will gradually learn how to use package managers to install development tools.

---

## Installing Visual Studio Code

Before writing software, we need a place to write our code.

A **code editor** is a specialized application designed for writing and editing source code.

Unlike ordinary word processors, code editors understand programming languages and provide features such as:

- Syntax highlighting
- Code completion
- Error detection
- Project management
- Extension support

Throughout this course, we will use **Visual Studio Code (VS Code)** because it is free, widely used in the software industry, and supports many programming languages.

### Windows

1. Visit the official Visual Studio Code website.
2. Download the Windows installer.
3. Run the installer.
4. Accept the license agreement.
5. Keep the default installation settings.
6. Complete the installation.
7. Launch Visual Studio Code.

### macOS

1. Visit the official Visual Studio Code website.
2. Download the macOS version.
3. Open the downloaded file.
4. Drag Visual Studio Code into the Applications folder.
5. Launch the application.

### Linux

Install Visual Studio Code using the package manager recommended by your Linux distribution or follow the installation guide provided on the official website.

### Verify Installation

Open Visual Studio Code.

If the application opens successfully, the installation was successful.

---

## Installing a Modern Web Browser

Software engineers spend a significant amount of time testing websites and web applications.

For this course, we recommend using one of the following modern browsers:

- Google Chrome
- Microsoft Edge
- Mozilla Firefox

These browsers include powerful developer tools that will become essential as you progress through the curriculum.

---

## Understanding the Terminal

Most beginners interact with computers using graphical interfaces.

Professional software engineers also use another powerful tool known as the **terminal**.

The terminal allows developers to communicate directly with the operating system by typing commands.

Instead of clicking buttons, developers can perform many tasks by entering commands.

Examples include:

- Creating folders.
- Navigating directories.
- Running programs.
- Installing software.
- Managing projects.

In the next lesson, you will begin learning how to use the terminal confidently.

---

## Opening Your Terminal

Every operating system includes a terminal application.

### Windows

Open **Windows Terminal** or **PowerShell** from the Start Menu.

### macOS

Open **Terminal** from the Applications folder or by searching with Spotlight.

### Linux

Open the Terminal application provided by your Linux distribution.

Do not worry if the terminal looks unfamiliar.

You will learn how to use it step by step in the next lesson.

---

## Creating Your First Workspace

A **workspace** is the location where you store your software projects.

Keeping all your projects in one location makes them easier to organize and manage.

In the next lesson, you will create your first workspace using terminal commands.

---

## Verifying Your Development Environment

Before moving forward, verify that:

- Visual Studio Code opens successfully.
- Your preferred web browser works correctly.
- Your terminal opens successfully.
- You have an internet connection.
- Your computer has sufficient storage space.

If all of these are working correctly, your development environment is ready for the next lesson.

---

## Troubleshooting Common Installation Problems

Sometimes software installation does not go as expected.

This is completely normal.

Professional software engineers regularly troubleshoot technical problems.

When you encounter an issue:

1. Read the error message carefully.
2. Confirm that you downloaded the software from its official website.
3. Restart the application if necessary.
4. Restart your computer.
5. Search the official documentation.
6. Ask your instructor if the problem persists.

Troubleshooting is an important software engineering skill.

Learning how to solve technical problems is just as valuable as learning how to write code.

---

# Practical Activity / Lab

## Preparing Your Development Environment

Complete the following tasks:

1. Identify your operating system.
2. Install Visual Studio Code.
3. Install a modern web browser if necessary.
4. Open your terminal.
5. Create a folder named `learnthencode` inside your Documents folder.
6. Open the folder in Visual Studio Code.
7. Verify that Visual Studio Code and your terminal both open successfully.

Record any problems you encountered and explain how you solved them.

---

# Key Takeaways

- A development environment is the collection of tools used to build software.
- Operating systems provide the foundation for software development.
- Download software only from official sources.
- Package managers simplify software installation.
- Visual Studio Code will be your primary code editor throughout this course.
- The terminal is an essential tool for every software engineer.
- Troubleshooting installation problems is part of becoming a software engineer.

---

# Summary

In this lesson, you learned:

- What a development environment is.
- Why operating systems are important.
- How to download software safely.
- What package managers do.
- How to install Visual Studio Code.
- Why developers use the terminal.
- How to verify that your computer is ready for software development.

Remember:

> **A well-prepared development environment allows you to focus on solving problems instead of fighting your tools.**

---

# Before You Continue

Before moving to the next lesson, make sure you can confidently:

- [ ] Explain what a development environment is.
- [ ] Identify your operating system.
- [ ] Download software safely.
- [ ] Explain the purpose of package managers.
- [ ] Open Visual Studio Code.
- [ ] Open your terminal.
- [ ] Verify that your development environment is ready.

If you are unsure about any of the above, review this lesson before continuing.

---

# What's Next?

Now that your computer is ready for software development, the next lesson introduces:

**The Command Line**

You will learn how software engineers communicate with their computers using terminal commands and begin navigating your development environment like a professional.