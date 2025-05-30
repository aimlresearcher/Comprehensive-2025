# ⚡ Interrupts in Operating Systems

## 🔍 What is an Interrupt?
An **interrupt** is a signal sent to the CPU by hardware or software indicating an event that needs immediate attention.

### 🧠 Purpose:
Interrupts pause the current process, save its state, and switch the CPU to run an **Interrupt Service Routine (ISR)** to handle the event.

---

## 🧩 Why Are Interrupts Needed?

### Without interrupts:
- The CPU must **poll** (continuously check) devices for events → inefficient.

### With interrupts:
- Devices notify the CPU **only when needed** → efficient multitasking and better performance.

---

## 🔧 Types of Interrupts

| Type                | Description                                            | Example                                      |
|---------------------|--------------------------------------------------------|----------------------------------------------|
| **Hardware Interrupt** | Generated by external devices via interrupt controller | Keyboard key press, mouse click              |
| **Software Interrupt** | Triggered by executing a system call                   | `int 0x80` in x86 Linux for system calls     |
| **Timer Interrupt**    | Issued by a hardware timer to enable preemptive multitasking | Used by OS to switch processes        |
| **I/O Interrupt**      | From I/O devices to signal completion of an operation  | Disk read complete                           |
| **Internal (Trap/Fault)** | Caused by an error or exception within the CPU         | Divide by zero, invalid memory access        |

---

## 🧠 Interrupt Handling Process

1. **Interrupt Signal Received**
2. **CPU finishes current instruction**
3. **CPU switches to kernel mode**
4. **Program Counter (PC)** and **CPU state** are saved
5. **CPU jumps to the Interrupt Service Routine (ISR)**
6. **ISR handles the event**
7. **CPU state is restored** and the previous process resumes

> ✅ **OS ensures** that interrupts are prioritized and can even be **nested** (high-priority interrupts can interrupt lower-priority ones).

## 🖼️ Visual: Interrupt Cycle

**Normal Execution → Interrupt Occurs → Save State → Run ISR → Restore State → Resume Execution**

---

## 🔃 Interrupt Vector Table

- A table stored in memory containing the addresses of all ISRs.
- Each type of interrupt has a **unique interrupt number** → used to index this table.

---

## 📋 Advantages of Interrupts

- Improves **CPU efficiency** (no polling).
- Enables **asynchronous I/O**.
- Allows **real-time response** to critical events.
- Supports **multitasking** and **time-sharing**.

---

## 📊 Summary Table

| Feature                 | Description                                      |
|-------------------------|--------------------------------------------------|
| **Interrupt**           | Signal to CPU that an event needs attention      |
| **ISR (Interrupt Handler)** | Function that handles specific interrupts     |
| **Interrupt Vector Table** | Stores addresses of all ISRs                  |
| **Preemptive Multitasking** | Enabled via timer interrupts                 |
| **Hardware vs Software**   | Hardware: from devices; Software: from programs |

