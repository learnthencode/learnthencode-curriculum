# Understanding Computers and Software

## Overview

Every software engineer builds software for computers, but understanding how computers work helps engineers make better decisions.

Before creating applications, it is important to understand the relationship between:

- Hardware.
- Software.
- Operating systems.
- Applications.
- Programming languages.

In this lesson, you will explore how computers execute instructions and how software interacts with the physical machine.

The goal is not to become a computer hardware expert.

The goal is to develop a mental model that helps you understand the environment where software lives.

---

## Learning Objectives

By the end of this lesson, you should be able to:

- Explain what a computer is.
- Describe the relationship between hardware and software.
- Explain how computers process information.
- Understand the purpose of an operating system.
- Explain the difference between applications and programs.
- Understand how software runs on a computer.

---

## Why This Matters

Software engineers create solutions that run on computers.

Without understanding the relationship between software and the machine it runs on, developers may struggle to answer important questions:

- Why does software need an operating system?
- Why does an application require memory?
- Why do different computers behave differently?
- Why do developers need different environments?

A strong engineer understands not only the code they write but also where that code executes.

---

# Sub-lessons

## What Is a Computer?

A computer is an electronic device that receives input, processes information, stores data, and produces output.

At its simplest, a computer follows this cycle:

```
Input
  ↓
Processing
  ↓
Storage
  ↓
Output
```

### Input

Input refers to information provided to a computer.

Examples:

- Keyboard typing.
- Mouse clicks.
- Touchscreen interaction.
- Camera images.
- Microphone recordings.

### Processing

Processing is the work performed by the computer to transform input into useful information.

The processor (CPU) performs instructions that tell the computer what actions to take.

### Storage

Storage allows computers to save information for later use.

Examples:

- Files.
- Applications.
- Photos.
- Documents.

### Output

Output is the information produced by a computer.

Examples:

- Displaying content on a screen.
- Playing audio.
- Printing documents.

---

## Hardware and Software

A computer is made of two major parts:

- Hardware.
- Software.

Together, they allow computers to perform useful tasks.

---

### Hardware

Hardware refers to the physical components of a computer that can be touched.

Examples:

- Processor (CPU).
- Memory (RAM).
- Storage devices.
- Keyboard.
- Monitor.
- Network devices.

#### CPU (Central Processing Unit)

The CPU is often called the "brain" of the computer.

It executes instructions and performs calculations required by software.

#### RAM (Memory)

RAM is temporary memory used by programs while they are running.

For example:

When you open a browser, the browser uses RAM to store information needed while you use it.

#### Storage

Storage keeps data even when the computer is turned off.

Examples:

- SSDs.
- Hard drives.

Storage contains:

- Operating systems.
- Applications.
- User files.

---

### Software

Software is a collection of instructions that tells hardware what to do.

Hardware without software cannot perform useful tasks.

Examples of software:

- Operating systems.
- Web browsers.
- Mobile applications.
- Games.
- Development tools.

The relationship can be represented as:

```
Software
    ↓
Controls
    ↓
Hardware
```

Software gives instructions, while hardware performs the actions.

---

## How Computers Process Information

Computers process information using instructions.

At a basic level:

```
Human Problem
      ↓
Software Solution
      ↓
Programming Instructions
      ↓
Computer Executes Instructions
      ↓
Result
```

Humans communicate with computers through programming languages.

Examples:

- JavaScript.
- Python.
- Java.
- C++.

However, computers do not directly understand these languages.

Computers ultimately understand machine instructions represented as binary:

```
0s and 1s
```

Programming languages allow humans to write instructions in a form that is easier to understand.

---

## Operating Systems Explained

An operating system is software that manages computer hardware and provides a platform for applications.

Without an operating system, using a computer would be extremely difficult.

Examples of operating systems:

- Windows.
- macOS.
- Linux.
- Android.
- iOS.

---

### Responsibilities of an Operating System

An operating system manages:

#### Hardware Resources

The operating system communicates with hardware components.

Examples:

- CPU usage.
- Memory allocation.
- Storage access.

#### Applications

The operating system provides an environment where applications can run.

#### Files

The operating system organizes and manages files and folders.

#### User Interaction

The operating system provides interfaces that allow users to interact with computers.

Examples:

- Desktop environments.
- Command-line interfaces.

---

## Applications and Programs

The terms application and program are often used interchangeably, but they can have slightly different meanings.

### Program

A program is a set of instructions designed to perform a task.

Example:

A calculator program performs mathematical operations.

### Application

An application is software designed to help users perform specific activities.

Examples:

- Web browsers.
- Banking applications.
- Learning platforms.

Applications are usually larger programs designed around user needs.

---

## How Software Runs on a Computer

When a developer writes code, the computer does not immediately understand it.

The process involves several layers:

```
Source Code
     ↓
Programming Language
     ↓
Compiler / Interpreter
     ↓
Operating System
     ↓
Hardware
     ↓
Result
```

---

### Source Code

Source code is the instructions written by developers.

Example:

```javascript
console.log("Hello World");
```

---

### Compiler and Interpreter

Programming languages require tools that translate instructions into a form computers can execute.

Two common approaches are:

### Compiler

A compiler translates an entire program before execution.

Examples:

- C.
- C++.

### Interpreter

An interpreter executes instructions while reading them.

Examples:

- JavaScript.
- Python.

---

### Operating System Layer

The operating system manages communication between software and hardware.

Applications usually do not communicate directly with hardware.

Instead:

```
Application
     ↓
Operating System
     ↓
Hardware
```

---

### Hardware Execution

Finally, the hardware performs the instructions.

The CPU processes instructions, memory stores temporary information, and storage saves permanent data.

---

# Practical Activity / Lab

## Explore Your Computer

Before becoming a developer, understand the machine you will use for development.

Document the following:

### Computer Information

Find:

- Operating system.
- Processor (CPU).
- Installed memory (RAM).
- Storage capacity.

### Software Information

Identify:

- Applications you frequently use.
- Your default web browser.
- Your file management system.

### Reflection Questions

Answer:

1. What operating system does your computer use?
2. Why do applications need an operating system?
3. What is the difference between hardware and software?
4. Why do developers need to understand the computers they build for?

---

# Key Takeaways

- Computers receive input, process information, store data, and produce output.
- Hardware refers to the physical components of a computer, while software consists of the instructions that control the hardware.
- Operating systems manage hardware resources and provide an environment for applications to run.
- Programs and applications work together with the operating system to perform useful tasks.
- Source code is translated into machine-executable instructions before hardware can execute it.

# Summary

In this lesson, you learned:

- Computers receive input, process information, store data, and produce output.
- Hardware refers to the physical components of a computer.
- Software provides instructions that control hardware.
- Operating systems manage hardware and provide environments for applications.
- Applications are programs designed to solve user problems.
- Software moves through several layers before producing results.

Remember:

> **Software does not exist separately from computers. Great software engineers understand both the instructions they write and the machines that execute them.**

---

# Before You Continue

Before moving to the next lesson, make sure you can confidently:

- [ ] Explain the difference between hardware and software.
- [ ] Describe how a computer processes information.
- [ ] Explain the purpose of an operating system.
- [ ] Differentiate applications from programs.
- [ ] Describe how source code becomes executable instructions.

If you are unsure about any of the above, review this lesson before continuing.

# What's Next?

Now that you understand computers and software, the next lesson will explore:

**The Software Development Journey**

You will learn how professional software engineers transform ideas and problems into real software products.