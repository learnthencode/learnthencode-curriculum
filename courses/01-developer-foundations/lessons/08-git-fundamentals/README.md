# Git Fundamentals

## Overview

In the previous lesson, you learned why software engineers use version control and how Git helps developers manage changes in software projects.

Now it is time to begin using Git.

Git is one of the most widely used tools in software engineering. Whether you are building personal projects, collaborating with a team, or contributing to open-source software, Git helps you track changes, organize your work, and confidently experiment without fear of losing progress.

In this lesson, you will install and configure Git, create your first Git repository, track changes, create commits, and view the history of your project.

The goal is simple:

> **Understand how Git works by using it to manage your own projects.**

---

# Learning Objectives

By the end of this lesson, you should be able to:

- Verify that Git is installed.
- Explain what a Git repository is.
- Configure Git with your name and email address.
- Create a Git repository.
- Check the status of a repository.
- Track changes using Git.
- Create commits.
- View commit history.
- Understand the basic Git workflow.

---

# Why This Matters

Professional software engineers rarely save code without version control.

Instead, they regularly record meaningful changes as they build software.

Git helps developers:

- Keep a complete history of their work.
- Recover previous versions.
- Experiment safely.
- Understand how projects evolve.
- Collaborate with other developers.

Learning Git is one of the most valuable skills you can develop as a software engineer.

---

# Sub-lessons

## Verifying Your Git Installation

Before using Git, confirm that it is installed correctly.

Open your terminal and run:

| Windows (PowerShell) | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `git --version` | `git --version` | Displays the installed Git version |

Example:

```text
git version 2.50.1
```

If Git displays its version number, your installation was successful.

If you receive an error saying Git is not recognized, return to **Lesson 4** and verify your installation.

---

## Configuring Git

Git records who creates each commit.

Before using Git, configure your identity.

### Configure Your Name

Replace `"Your Name"` with your own name.

| Windows | macOS / Linux |
|----------|---------------|
| `git config --global user.name "Your Name"` | `git config --global user.name "Your Name"` |

Example:

```bash
git config --global user.name "Yahya Mohamed"
```

---

### Configure Your Email Address

Replace the email below with the same email you use for GitHub.

| Windows | macOS / Linux |
|----------|---------------|
| `git config --global user.email "your@email.com"` | `git config --global user.email "your@email.com"` |

Example:

```bash
git config --global user.email "yahya@example.com"
```

---

### Verify Your Configuration

Check your Git configuration.

| Windows | macOS / Linux | Purpose |
|----------------------|---------------|---------|
| `git config --list` | `git config --list` | Displays your Git configuration |

Example output:

```text
user.name=Yahya Mohamed
user.email=yahya@example.com
```

---

## What Is a Repository?

A repository (or **repo**) is a project managed by Git.

Think of it as a project folder with memory.

Git remembers every important change made inside the repository.

---

## Creating Your First Repository

Navigate to the **developer-foundations** folder you created in Lesson 6.

Initialize Git.

| Windows | macOS / Linux | Purpose |
|----------|---------------|---------|
| `git init` | `git init` | Creates a new Git repository |

Example output:

```text
Initialized empty Git repository...
```

Git creates a hidden directory named:

```text
.git
```

This directory stores your project's version history.

Never delete the `.git` directory unless you intentionally want to remove Git from the project.

---

## Checking Repository Status

Git can tell you the current state of your repository.

Run:

| Windows | macOS / Linux | Purpose |
|----------|---------------|---------|
| `git status` | `git status` | Shows the current repository status |

Initially, Git reports that no commits have been made.

As you work, `git status` becomes one of the most frequently used Git commands.

Professional developers use it constantly.

---

## Understanding the Git Workflow

Git follows a simple workflow.

```text
Working Directory
        │
        ▼
Staging Area
        │
        ▼
Repository (Commit History)
```

The process looks like this:

1. Create or modify files.
2. Stage the changes.
3. Commit the changes.

---

## Staging Files

Git does not automatically include every change in the next commit.

Instead, you choose which changes should be recorded.

Stage all changes:

| Windows | macOS / Linux | Purpose |
|----------|---------------|---------|
| `git add .` | `git add .` | Stages all changes |

Stage a single file:

```bash
git add README.md
```

---

## Creating Your First Commit

After staging your files, create a commit.

| Windows | macOS / Linux | Purpose |
|----------|---------------|---------|
| `git commit -m "Initial commit"` | `git commit -m "Initial commit"` | Creates a commit |

A commit message should briefly describe the changes.

Good examples:

```text
Initial commit
Add project documentation
Create login page
Fix navigation bug
```

Avoid vague messages such as:

```text
Update
Changes
Stuff
Final
```

Good commit messages make project history easier to understand.

---

## Viewing Commit History

Every commit becomes part of your project's history.

View your commit history.

| Windows | macOS / Linux | Purpose |
|----------|---------------|---------|
| `git log` | `git log` | Displays commit history |

Example:

```text
commit 8f2b1...

Author: Yahya Mohamed

Date:

    Initial commit
```

---

## Understanding Git Status

Throughout development, remember this simple workflow.

```text
Modify Files

      ↓

git status

      ↓

git add

      ↓

git commit

      ↓

Repeat
```

This cycle forms the foundation of everyday Git usage.

---

# Practical Activity / Lab

## Create Your First Git Repository

Complete the following steps.

1. Navigate to your `developer-foundations` project.
2. Verify Git is installed.
3. Configure your name.
4. Configure your email.
5. Initialize a Git repository.
6. Create a `README.md` file if one does not already exist.
7. Check the repository status.
8. Stage all files.
9. Create your first commit.
10. View the commit history.

Reflect on the following questions.

1. Why does Git require commits?
2. Why are commit messages important?
3. Why should developers check `git status` frequently?

---

# Key Takeaways

- Git tracks changes in software projects.
- Every Git project is stored in a repository.
- Commits record project history.
- The staging area allows developers to choose which changes to record.
- `git status` is one of the most important Git commands.
- Good commit messages improve project history.

---

# Summary

In this lesson, you learned:

- How to verify Git installation.
- How to configure Git.
- How to create a repository.
- How to check repository status.
- How to stage files.
- How to create commits.
- How to view project history.
- The basic Git workflow used by professional developers.

Remember:

> **Every great software project is built one meaningful commit at a time.**

---

# Before You Continue

Before moving to the next lesson, make sure you can confidently:

- [ ] Verify your Git installation.
- [ ] Configure Git with your name and email.
- [ ] Create a Git repository.
- [ ] Check repository status.
- [ ] Stage files.
- [ ] Create commits.
- [ ] View commit history.
- [ ] Explain the Git workflow.

If you are unsure about any of the above, review this lesson before continuing.

---

# What's Next?

Now that you know how to use Git locally, the next lesson introduces:

**GitHub and Collaboration**

You will learn how to connect your local Git repositories to GitHub, publish projects online, collaborate with other developers, and contribute to software projects using modern Git workflows.