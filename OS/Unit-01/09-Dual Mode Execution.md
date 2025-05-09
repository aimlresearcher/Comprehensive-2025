# 🔐 Dual Mode Execution

## 🎯 Purpose

Dual mode execution is a fundamental concept in modern operating systems that ensures **system security and stability** by separating user activities from OS operations.

---

## 🧩 What is Dual Mode?

The CPU operates in two distinct modes to distinguish between executing user-level code (applications) and kernel-level code (OS services):

| Mode        | Description                                | Example                        |
|-------------|--------------------------------------------|--------------------------------|
| **User Mode**   | Restricted mode; for user applications     | Running MS Word, Browser       |
| **Kernel Mode** | Privileged mode; full access to all hardware and memory | Performing file I/O, scheduling |

---

## 🔧 How It Works

- A **mode bit** (typically a single flag in the CPU) indicates the current mode:
  - `0` = **Kernel Mode**
  - `1` = **User Mode**
- The system boots in **kernel mode** and switches to **user mode** before launching user applications.
- Any critical operation (like accessing I/O devices, memory management, or process control) requires switching to **kernel mode**, typically via system calls or interrupts.

---

## 📜 Transition Between Modes

| Situation                          | Transition          | Example                        |
|------------------------------------|----------------------|--------------------------------|
| User program calls OS service      | User → Kernel        | `read()`, `write()`, `fork()`  |
| Hardware interrupt (e.g., I/O done)| User/Kernel → Kernel | Disk finished reading data     |
| OS finishes executing service      | Kernel → User        | Return to application          |

---

## 🚨 Why Dual Mode is Important

### ✅ Protection
Prevents user programs from accidentally or maliciously damaging the OS or hardware.

### ✅ Stability
Keeps the system operational even if an application crashes.

### ✅ Controlled Access
Only the OS (in kernel mode) can execute **privileged instructions** (e.g., setting interrupt vectors, accessing device registers).

### ✅ Isolation
Prevents faulty or unauthorized code from interfering with other applications or the OS.

---

## ⚠️ Privileged Instructions

Certain instructions can only be executed in **kernel mode**, such as:

- Disabling/enabling interrupts
- Direct hardware I/O
- Changing mode bits
- Managing memory or process tables

> If a **user-mode** program attempts these, the OS will **trap** and possibly **terminate** it.

---

## 🧠 Example in Action

1. User opens a file (**user mode**).
2. System call `open()` is made → switches to **kernel mode**.
3. OS accesses the file system and returns a file handle.
4. Control is passed back to **user mode**.

---

## 📊 Summary Table

| Feature                        | User Mode        | Kernel Mode       |
|--------------------------------|------------------|-------------------|
| **Access Level**               | Limited          | Full system access|
| **Used By**                    | Applications     | Operating System core |
| **Can Execute Privileged Instructions?** | ❌ No         | ✅ Yes            |
| **System Calls Allowed?**      | ✅ (via transition) | ✅ Native       |
| **Example Task**               | Running Calculator App | Handling disk I/O or memory allocation |
