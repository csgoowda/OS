# Operating System Fundamentals

Before learning OS interview topics, first understand:

> **Why do we even need an Operating System?**

Without an OS, a computer is just hardware.

You would have to manually tell the CPU, RAM, keyboard, and storage how to communicate.

The OS acts as a **manager** between the user and hardware.

```text
User
 ↓
Operating System
 ↓
Hardware
```

---

# What is an Operating System?

An Operating System (OS) is system software that manages computer hardware, software resources, and provides services to programs.

### Examples

* Windows
* Linux
* macOS
* Android

---

# Real-Life Example

Imagine a college.

### Principal

Manages everything.

### Students

Request resources.

### Staff

Perform tasks.

Similarly:

### OS

Manages everything.

### Programs

Request resources.

### Hardware

Provides resources.

---

# Functions of an Operating System

---

## 1. Process Management

The OS manages running programs.

Example:

You open:

* Chrome
* VS Code
* Spotify

OS decides:

* Which program runs first
* How much CPU each gets

---

## 2. Memory Management

OS manages RAM.

Example:

RAM = 8 GB

Open:

* Chrome → 2 GB
* VS Code → 1 GB
* Spotify → 500 MB

OS allocates memory.

---

## 3. File Management

OS manages files and folders.

Example:

```text
Documents/
Pictures/
Videos/
```

Without OS, organizing files would be impossible.

---

## 4. Device Management

OS controls:

* Keyboard
* Mouse
* Printer
* USB

Through device drivers.

---

## 5. Security

OS provides:

* Login passwords
* User permissions
* Access control

---

# Types of Operating Systems

---

# 1. Batch Operating System

Jobs are collected and executed in batches.

Example:

Old payroll systems.

---

### Advantage

High throughput.

### Disadvantage

No direct user interaction.

---

# 2. Multiprogramming OS

Multiple programs stay in memory simultaneously.

Example:

```text
Program A
Program B
Program C
```

CPU switches among them.

---

### Goal

Keep CPU busy.

---

# 3. Multitasking OS

Multiple applications run apparently at the same time.

Example:

```text
Chrome
VS Code
Spotify
```

Running together.

---

### Example

Windows and Linux.

---

# 4. Multiuser OS

Multiple users share the same system.

Example:

Linux server.

Many users connected simultaneously.

---

# 5. Real-Time Operating System (RTOS)

Used where response time is critical.

Examples:

* Air Traffic Control
* Medical Equipment
* Robotics

---

### Example

Pacemaker.

Response delay could be dangerous.

---

# What is a Kernel?

Kernel is the core part of the Operating System.

It directly interacts with hardware.

---

### Architecture

```text
User
 ↓
Application
 ↓
Kernel
 ↓
Hardware
```

---

# Responsibilities of Kernel

* Memory Management
* Process Management
* Device Management
* System Calls

---

# Real-Life Example

Think of Kernel as:

```text
Prime Minister
```

Every important decision goes through it.

---

# What is a Shell?

Shell is an interface between user and OS.

It accepts commands from users.

---

### Example

Linux Terminal

```bash
ls
mkdir
cd
```

These commands are interpreted by the shell.

---

# Shell vs Kernel

| Shell            | Kernel            |
| ---------------- | ----------------- |
| User interface   | Core of OS        |
| Accepts commands | Executes commands |
| Outer layer      | Inner layer       |

---

# System Calls

Applications cannot directly access hardware.

They ask the OS through system calls.

---

### Example

Suppose:

```cpp
open("file.txt");
```

Application requests:

```text
Open file
```

OS performs the operation.

---

# Why System Calls?

Security.

Without them:

Applications could directly manipulate hardware.

---

# User Mode vs Kernel Mode

One of the most asked interview questions.

---

# User Mode

Applications run here.

Examples:

* Chrome
* VS Code
* WhatsApp

Restrictions exist.

Cannot directly access hardware.

---

# Kernel Mode

Operating system runs here.

Full access to:

* CPU
* Memory
* Devices

---

# User Mode vs Kernel Mode

| User Mode        | Kernel Mode   |
| ---------------- | ------------- |
| Limited access   | Full access   |
| Applications run | OS runs       |
| More secure      | More powerful |

---

# Booting Process

What happens when you press the power button?

---

## Step 1

Power ON.

---

## Step 2

BIOS/UEFI starts.

Checks hardware.

---

## Step 3

Bootloader loads.

---

## Step 4

Kernel loads into memory.

---

## Step 5

Operating System starts.

---

# BIOS vs UEFI

| BIOS             | UEFI          |
| ---------------- | ------------- |
| Older            | Newer         |
| Slower           | Faster        |
| Limited features | More features |

---

# Most Important Interview Questions

## Easy

### What is an Operating System?

An Operating System is system software that manages hardware and software resources.

---

### Why is OS needed?

To manage hardware, software, memory, files, and processes.

---

### What are the functions of OS?

* Process Management
* Memory Management
* File Management
* Device Management
* Security

---

### What is a Kernel?

The core component of an OS that directly interacts with hardware.

---

### What is a Shell?

An interface between user and operating system.

---

## Medium

### Shell vs Kernel?

| Shell            | Kernel            |
| ---------------- | ----------------- |
| Interface        | Core              |
| Accepts commands | Executes commands |

---

### What are System Calls?

Mechanism by which applications request services from the OS.

---

### What is User Mode?

Restricted mode where applications run.

---

### What is Kernel Mode?

Privileged mode where the OS runs.

---

## Hard

### Why can't applications directly access hardware?

For security and resource management.

---

### Explain the booting process.

Power On → BIOS/UEFI → Bootloader → Kernel → OS.

---

### Why is Kernel important?

Because it manages CPU, memory, devices, and system resources.

---

# End of Day 10 Target

You should clearly understand:

✅ What is OS

✅ Functions of OS

✅ Types of OS

✅ Kernel

✅ Shell

✅ System Calls

✅ User Mode vs Kernel Mode

✅ Booting Process

These topics build the foundation for Day 11, where you'll learn the most frequently asked OS interview topic:

**Process, Thread, Process States, Context Switching, and CPU Scheduling.**
