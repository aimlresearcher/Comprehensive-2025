# 🧑‍💻 1. Single-User vs Multi-User Operating Systems

## 🔹 Single-User OS
- Supports **one user** at a time.
- Designed for **personal computers** or **mobile devices**.
- **Examples:** Windows 10, macOS, Android (single user interface, though may support multiple profiles).

### Key Features:
- Simplicity  
- Direct resource access  
- No need for access control between users  

---

## 🔹 Multi-User OS
- Allows **multiple users** to access system resources **simultaneously**.
- Requires **user authentication**, **access control**, and **resource scheduling**.
- **Examples:** UNIX, Linux, mainframe OSes.

### Key Features:
- Process isolation  
- Security and permission management  
- Concurrent execution  
- Efficient CPU and memory management  

---

# ⚙️ 2. Services Provided by Operating Systems

Operating systems provide a set of standard services to:

- Simplify application programming  
- Abstract hardware  
- Protect system resources  

## 🔧 Common OS Services

| Service               | Description                                      |
|------------------------|--------------------------------------------------|
| **Program Execution**  | Load and run programs efficiently.               |
| **I/O Operations**     | Manage input/output with devices (keyboard, disk, etc.). |
| **File System Management** | Create, delete, and access files and directories. |
| **Memory Management**  | Allocate and deallocate memory to processes.     |
| **Process Management** | Create, schedule, and terminate processes.       |
| **Security & Protection** | Control user access and enforce resource isolation. |
| **Networking**         | Enable communication between processes on different systems. |
| **Error Detection**    | Identify and respond to hardware and software failures. |

---

# 📞 3. System Calls

## 🔹 What is a System Call?
A **system call** is a programmatic way for user programs to **request services from the operating system’s kernel**.

> 🧠 Think of it as a **"doorway"** to access kernel-mode operations from user-mode programs.

## 🔹 Common Types of System Calls

| Type                  | Example Calls                        | Description                         |
|------------------------|--------------------------------------|-------------------------------------|
| **Process Control**    | `fork()`, `exec()`, `exit()`         | Create/terminate processes          |
| **File Management**    | `open()`, `read()`, `write()`, `close()` | File I/O operations              |
| **Device Management**  | `ioctl()`, `read()`, `write()`       | Interact with hardware devices      |
| **Information Maintenance** | `getpid()`, `alarm()`, `time()` | Monitor system status               |
| **Communication**      | `pipe()`, `shmget()`, `send()`, `recv()` | IPC (inter-process communication) |

---

# 🐚 4. Shell Management

## 🔹 What is a Shell?
A **shell** is a command-line interpreter that allows users to **interact with the OS using commands**.  
It serves as a **bridge between the user and the kernel**.

## 🔹 Shell Types

**Command Line Shells:**
- `bash` (Bourne Again SHell)
- `sh`, `csh`, `zsh`

**Graphical Shells:**
- Windows Explorer  
- macOS Finder  

## 🔹 Responsibilities of a Shell
- Interpret and execute user commands  
- Manage I/O redirection (`>`, `<`, `>>`)  
- Handle piping (`|`) to connect commands  
- Launch and manage processes (e.g., `ls`, `ps`, `kill`)  

## 🔹 Shell Scripting
- Automates **repetitive tasks** using scripts.
- Example:
```bash
#!/bin/bash
echo "Hello, $USER"
date
```
## 📝 Summary Table

| Concept         | Key Points                                                                 |
|------------------|---------------------------------------------------------------------------|
| **Single-User OS** | One user at a time, personal use, simpler resource control               |
| **Multi-User OS**  | Supports many users simultaneously, secure and concurrent access         |
| **OS Services**    | Execution, I/O, file/memory/process management, security                 |
| **System Calls**   | Interface to kernel services, e.g., `read()`, `fork()`, `open()`         |
| **Shell**          | Command interpreter, user-to-kernel interface, supports scripting        |
