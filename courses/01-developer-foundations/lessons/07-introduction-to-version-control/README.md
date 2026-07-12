# Introduction to Version Control

## Overview

Software is constantly changing.

Developers add new features, fix bugs, improve performance, and update existing functionality. Without a way to track these changes, software projects can quickly become difficult to manage.

Imagine spending several days working on a project only to accidentally delete an important file or introduce a bug that breaks your application.

Without a record of previous versions, recovering your work can be extremely difficult.

Professional software engineers solve this problem using **version control**.

Version control allows developers to record changes, restore previous versions, experiment safely, and collaborate with others without losing their work.

In this lesson, you will learn what version control is, why it is essential, and how it has transformed modern software development.

The goal is simple:

> **Understand why version control exists before learning how to use Git.**

---

## Learning Objectives

By the end of this lesson, you should be able to:

- Explain what version control is.
- Describe the problems version control solves.
- Differentiate between manual and automated version control.
- Explain the different types of version control systems.
- Understand why Git was created.
- Define repositories and commits conceptually.
- Explain how version control improves collaboration.

---

## Why This Matters

Software projects rarely remain the same.

Developers constantly make changes.

Without a reliable way to manage those changes, problems such as these become common:

- Accidentally deleting important files.
- Overwriting someone else's work.
- Forgetting what changed.
- Introducing bugs with no way to recover.
- Maintaining multiple confusing copies of the same project.

Version control solves these problems.

It allows developers to work confidently, knowing they can review previous work, restore older versions, and collaborate effectively.

Today, version control is one of the most important skills every software engineer must learn.

---

# Sub-lessons

## The Problem Before Version Control

Before version control systems became popular, developers often created multiple copies of the same project.

For example:

```text
calculator
calculator-new
calculator-final
calculator-final-v2
calculator-final-v3
calculator-final-v3-fixed
calculator-final-final
calculator-final-final-REAL
```

As projects grew, this approach became confusing.

Developers struggled to answer questions such as:

- Which version is the newest?
- Which version contains the latest bug fix?
- Which version should I continue working on?
- Can I recover changes I made yesterday?

Managing projects this way wastes time and increases the likelihood of mistakes.

---

## What Is Version Control?

Version control is a system that records changes made to files over time.

Instead of creating multiple copies of a project, version control stores the history of every change.

This allows developers to:

- Track changes.
- Restore previous versions.
- Compare different versions.
- Experiment safely.
- Collaborate with others.

Think of version control as a detailed timeline of your project.

Every important change is recorded.

---

## Manual Version Control vs Automated Version Control

### Manual Version Control

Many beginners manage projects manually by creating multiple folders.

Example:

```text
website
website-v2
website-v3
website-final
website-final-new
```

Although simple, this method becomes difficult to manage as projects grow.

Problems include:

- Duplicate files.
- Confusing folder names.
- Lost work.
- No detailed history.

---

### Automated Version Control

Automated version control systems record changes automatically.

Instead of creating duplicate folders, developers save changes as versions within the same project.

Benefits include:

- Organized history.
- Easier recovery.
- Better collaboration.
- Reduced duplication.

---

## Types of Version Control Systems

There are three common types of version control systems.

---

### Local Version Control

A local version control system stores the history of a project on a single computer.

```text
Developer
     │
     ▼
Local Repository
```

Advantages:

- Simple.
- Fast.

Limitations:

- Difficult to collaborate.
- History may be lost if the computer fails.

---

### Centralized Version Control

A centralized system stores project history on a central server.

```text
Developer A
      │
Developer B
      │
Developer C
      ▼
Central Server
```

Advantages:

- Easier collaboration.
- Central backup.

Limitations:

- If the server becomes unavailable, development may stop.

---

### Distributed Version Control

Modern software engineering primarily uses distributed version control.

Each developer has a complete copy of the project's history.

```text
Developer A ◄────► Repository

Developer B ◄────► Repository

Developer C ◄────► Repository
```

Advantages:

- Every developer has a complete backup.
- Better collaboration.
- Faster development.
- Improved reliability.

Git is the world's most popular distributed version control system.

---

## Why Git Was Created

As software projects became larger and more complex, developers needed a faster and more reliable version control system.

Git was created to solve this problem.

Git allows developers to:

- Track every change.
- Restore previous versions.
- Work offline.
- Collaborate with teams.
- Experiment without fear of losing work.

Today, Git is used by millions of developers and organizations around the world.

---

## Key Version Control Concepts

Before learning Git commands, it is important to understand a few key concepts.

### Repository

A **repository** (often called a **repo**) is a project that is managed using version control.

Think of a repository as a project folder with memory.

It remembers every important change made to the project.

---

### Commit

A **commit** is a saved snapshot of your project.

Each commit records:

- What changed.
- Who made the change.
- When the change was made.
- A message describing the change.

Over time, commits create a complete history of the project.

---

### History

Every commit is stored in chronological order.

Example:

```text
Commit 1
     │
     ▼
Commit 2
     │
     ▼
Commit 3
     │
     ▼
Current Version
```

Developers can review previous commits whenever necessary.

---

## Working Together Using Version Control

Imagine three developers working on the same project.

Without version control:

- Files may overwrite each other.
- Important changes can be lost.
- Collaboration becomes difficult.

With version control:

- Every developer works independently.
- Changes are recorded.
- Work can be combined safely.
- Previous versions remain available.

Version control enables teams to build software together efficiently.

---

## Version Control in Everyday Life

Even outside software engineering, many people already practice a form of version control.

Examples include:

- Saving multiple versions of a school assignment.
- Keeping different drafts of a report.
- Editing presentations before submitting them.

Version control systems improve this process by automatically managing every revision.

Instead of creating:

```text
Essay
Essay-New
Essay-Final
Essay-Final-Updated
Essay-Final-Real
```

A version control system stores every revision inside one organized project.

---

# Practical Activity / Lab

## Reflect on Your Own Workflow

Think about a document or school assignment you have edited multiple times.

Answer the following questions:

1. How did you keep track of different versions?
2. Have you ever accidentally overwritten important work?
3. How could version control have helped?
4. Why do you think software companies rely on version control?

Record your answers in your learning journal.

---

# Key Takeaways

- Software projects constantly change.
- Version control records every important change.
- Manual file versioning becomes difficult as projects grow.
- Automated version control systems provide a structured project history.
- Git is a distributed version control system.
- Repositories store projects, while commits record changes.
- Version control makes collaboration safer and more efficient.

---

# Summary

In this lesson, you learned:

- Why version control exists.
- The problems it solves.
- The different types of version control systems.
- Why Git became the industry standard.
- The concepts of repositories, commits, and project history.
- How version control improves collaboration.

Remember:

> **Version control is not just about saving code—it is about understanding the history of a project and giving developers the confidence to make changes safely.**

---

# Before You Continue

Before moving to the next lesson, make sure you can confidently:

- [ ] Explain what version control is.
- [ ] Describe the problems it solves.
- [ ] Differentiate between manual and automated version control.
- [ ] Explain the three types of version control systems.
- [ ] Define a repository.
- [ ] Define a commit.
- [ ] Explain why Git is the industry standard.

If you are unsure about any of the above, review this lesson before continuing.

---

# What's Next?

Now that you understand why version control exists, the next lesson introduces:

**Git Fundamentals**

You will install and configure Git, create your first repository, track changes, create commits, view project history, and begin using Git to manage your own software projects.