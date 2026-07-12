# GitHub and Collaboration

## Overview

In the previous lesson, you learned how to use Git locally to track changes, create commits, and manage the history of your projects.

However, software development is rarely done completely alone.

Professional developers need a way to store their projects online, share their work with others, and collaborate with team members across different locations.

This is where GitHub comes in.

GitHub is a platform that hosts Git repositories and provides tools that help developers collaborate, review code, manage projects, and contribute to software communities.

Before your computer can communicate with GitHub securely, you also need to understand authentication.

In this lesson, you will learn how GitHub works, how to connect Git with GitHub, how SSH authentication allows secure communication, how to publish projects online, and how developers collaborate using modern workflows.

The goal is simple:

> **Understand how developers use GitHub to securely share, collaborate, and build software together.**

---

# Learning Objectives

By the end of this lesson, you should be able to:

- Explain the difference between Git and GitHub.
- Understand local and remote repositories.
- Explain how authentication allows GitHub communication.
- Understand the purpose of SSH keys.
- Generate an SSH key.
- Add an SSH key to GitHub.
- Test an SSH connection.
- Create a GitHub repository.
- Connect a local Git repository to GitHub.
- Push code to GitHub.
- Pull updates from GitHub.
- Clone repositories.
- Explain the purpose of GitHub Issues.
- Explain the purpose of Pull Requests.
- Understand basic collaboration workflows.

---

# Why This Matters

Writing software is often a team effort.

A developer may work with:

- Other developers.
- Designers.
- Product managers.
- Test engineers.
- Open-source contributors.

Without a platform for sharing and managing code, collaboration becomes difficult.

GitHub provides developers with a central place to:

- Store projects.
- Share code.
- Review changes.
- Discuss improvements.
- Work together.

Authentication ensures that only authorized users can access and modify projects.

Learning GitHub helps you participate in real software development workflows.

---

# Sub-lessons

# Git vs GitHub

Although Git and GitHub are often mentioned together, they are different tools.

---

## What Is Git?

Git is a version control system installed on your computer.

Git helps you:

- Track changes.
- Create commits.
- Manage project history.
- Work with repositories.

Git works locally.

Example:

```text
Your Computer

Project Folder
      |
      |
     Git
      |
      |
Commit History
```

---

## What Is GitHub?

GitHub is an online platform that hosts Git repositories.

GitHub allows developers to:

- Store projects online.
- Share code.
- Collaborate with others.
- Review changes.

Example:

```text
Your Computer

Git Repository

        |
        |
        ▼

GitHub Repository
```

---

# Local vs Remote Repositories

A repository on your computer is called a **local repository**.

A repository stored online is called a **remote repository**.

Example:

```text
Local Repository

Your Computer
      |
      |
      ▼
    Git


Remote Repository

GitHub
      |
      |
      ▼
    Online Storage
```

Developers use Git commands to move changes between local and remote repositories.

---

# Understanding GitHub Authentication

Before your computer can communicate with GitHub, GitHub needs to verify your identity.

This process is called **authentication**.

Authentication answers the question:

> "Is this person allowed to access this GitHub account?"

GitHub supports different authentication methods.

The method introduced in this course is **SSH authentication**.

---

# What Is SSH?

SSH stands for **Secure Shell**.

SSH allows computers to communicate securely over a network.

For GitHub, SSH allows your computer to prove its identity without repeatedly entering your username and password.

SSH uses a pair of keys:

- Public key.
- Private key.

---

## Public Key

The public key is shared with GitHub.

Example:

```text
id_ed25519.pub
```

GitHub stores this key to recognize your computer.

---

## Private Key

The private key stays on your computer.

Example:

```text
id_ed25519
```

Never share your private key.

Anyone with access to your private key may be able to authenticate as you.

---

The relationship looks like this:

```text
Your Computer

Private Key

      |
      |
      ▼

Secure Authentication

      |
      |
      ▼

GitHub

Public Key
```

---

# Creating an SSH Key

You only need to create an SSH key once on each computer.

Use the instructions for your operating system.

---

## Windows

Open PowerShell or Git Bash.

Run:

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Replace the email with the email connected to your GitHub account.

Example:

```bash
ssh-keygen -t ed25519 -C "student@example.com"
```

When asked where to save the key, press:

```text
Enter
```

When asked for a passphrase, press:

```text
Enter
```

Press Enter again to confirm an empty passphrase.

---

## macOS

Open Terminal.

Run:

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Follow the prompts.

---

## Linux

Open Terminal.

Run:

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

Follow the prompts.

---

# Finding Your SSH Key

Your SSH keys are stored inside the `.ssh` folder.

---

## Windows

```powershell
dir ~/.ssh
```

---

## macOS/Linux

```bash
ls ~/.ssh
```

You should see:

```text
id_ed25519
id_ed25519.pub
```

Remember:

```text
id_ed25519

Private key
Keep secret.


id_ed25519.pub

Public key
Share with GitHub.
```

---

# Adding Your SSH Key to GitHub

First, copy your public key.

---

## Windows

Run:

```powershell
cat ~/.ssh/id_ed25519.pub | clip
```

---

## macOS

Run:

```bash
pbcopy < ~/.ssh/id_ed25519.pub
```

---

## Linux

Run:

```bash
cat ~/.ssh/id_ed25519.pub
```

Copy the displayed text.

---

Now add the key to GitHub:

1. Open GitHub.
2. Click your profile picture.
3. Select **Settings**.
4. Select **SSH and GPG keys**.
5. Click **New SSH key**.
6. Enter a title.

Example:

```text
Personal Laptop
```

7. Paste your public key.
8. Click **Add SSH key**.

---

# Testing Your SSH Connection

Verify that GitHub recognizes your computer.

Run:

```bash
ssh -T git@github.com
```

Successful output:

```text
Hi username! You've successfully authenticated, but GitHub does not provide shell access.
```

Your SSH connection is now ready.

---

# Creating a GitHub Repository

A remote repository is the online version of your project.

Follow these steps:

1. Sign in to GitHub.
2. Select **New Repository**.
3. Enter a repository name.
4. Choose public or private visibility.
5. Create the repository.

GitHub will provide instructions for connecting your local project.

---

# Connecting Git and GitHub

Your local repository does not automatically know about GitHub.

You need to add a remote repository.

The default remote name is:

```text
origin
```

---

Add the remote using the SSH URL:

```bash
git remote add origin git@github.com:username/project-name.git
```

---

Check your remote:

```bash
git remote -v
```

Example:

```text
origin git@github.com:username/project-name.git
```

---

# Pushing Code to GitHub

Pushing sends your local commits to GitHub.

Workflow:

```text
Local Repository

        |
        |
        ▼

GitHub Repository
```

Run:

```bash
git push -u origin main
```

After the first push:

```bash
git push
```

---

# Pulling Updates from GitHub

Pulling downloads changes from GitHub.

Run:

```bash
git pull
```

Developers commonly pull before starting work.

---

# Cloning Repositories

Cloning creates a local copy of an existing GitHub repository.

Run:

```bash
git clone git@github.com:username/project-name.git
```

Common reasons to clone:

- Joining an existing project.
- Contributing to open-source software.
- Downloading your projects on another computer.

---

# GitHub Issues

GitHub Issues help teams track work.

Developers use issues to record:

- Bugs.
- Feature requests.
- Improvements.
- Questions.

Example:

```text
Issue:

Login button does not work

Description:

Users cannot submit the login form.
```

---

# Pull Requests

A Pull Request (PR) is a request to add changes to a project.

Instead of directly changing the main project, developers:

1. Make changes.
2. Push their work.
3. Create a Pull Request.
4. Ask others to review.
5. Merge approved changes.

Workflow:

```text
Developer

      ↓

Changes

      ↓

Pull Request

      ↓

Code Review

      ↓

Project
```

---

# Collaboration Workflow

A simplified workflow looks like this:

```text
1. Receive a task

        ↓

2. Update local project

        ↓

3. Make changes

        ↓

4. Create commits

        ↓

5. Push changes to GitHub

        ↓

6. Review changes

        ↓

7. Update project
```

---

# Practical Activity / Lab

## Publish Your First Project on GitHub

Complete the following steps:

1. Create a GitHub account if you do not already have one.
2. Create an SSH key.
3. Add your SSH key to GitHub.
4. Test your SSH connection.
5. Create a GitHub repository.
6. Connect your local repository using SSH.
7. Push your project to GitHub.
8. Make a small change locally.
9. Create a commit.
10. Push the update.

---

## Reflection Questions

Answer the following questions:

1. What is the difference between Git and GitHub?
2. Why does GitHub require authentication?
3. What is the purpose of an SSH key?
4. Why should a private key never be shared?
5. What problem do Pull Requests solve?

Record your answers in your learning journal.

---

# Key Takeaways

- Git manages changes locally.
- GitHub hosts Git repositories online.
- Authentication allows secure communication with GitHub.
- SSH keys provide secure authentication.
- Public keys are shared with GitHub while private keys remain secret.
- `git push` uploads changes.
- `git pull` downloads updates.
- `git clone` creates local copies of repositories.
- Issues and Pull Requests support collaboration.

---

# Summary

In this lesson, you learned:

- The difference between Git and GitHub.
- How remote repositories work.
- How SSH authentication works.
- How to create and add SSH keys.
- How to connect Git with GitHub.
- How to push and pull projects.
- How developers collaborate using GitHub features.

Remember:

> **Git helps developers manage changes. GitHub helps developers securely share those changes and collaborate with others.**

---

# Before You Continue

Before moving to the next lesson, make sure you can confidently:

- [ ] Explain Git vs GitHub.
- [ ] Explain local and remote repositories.
- [ ] Create an SSH key.
- [ ] Add an SSH key to GitHub.
- [ ] Test your GitHub connection.
- [ ] Push code to GitHub.
- [ ] Pull updates.
- [ ] Clone repositories.
- [ ] Explain Issues and Pull Requests.

If you are unsure about any of the above, review this lesson before continuing.

---

# What's Next?

Now that you understand GitHub and collaboration, the next lesson combines everything you have learned into a complete professional development workflow.

You will learn how developers start projects, organize their work, write documentation, track changes, publish projects, and maintain software professionally.

**Professional Developer Workflow**