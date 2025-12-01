# Operating Systems – Assignment 4

This repository contains 5 Python programs demonstrating advanced Operating System concepts such as process creation, multiprocessing, inter-process communication, scheduling, and virtualization detection.

Each task is stored in a separate Python file for clarity and easy execution.

---

## 📌 Task 1 — Batch Script Runner

**File:** `task1.py`

This program:
- Stores multiple Python script filenames in a list  
- Executes them sequentially using `subprocess.call()`  
- Acts as a simple batch job executor or automation script  

Useful for simulating automated OS-level task execution.

---

## 📌 Task 2 — System Startup Simulation (Multiprocessing)

**File:** `task2.py`

Features:
- Demonstrates multiprocessing using Python’s `multiprocessing` module  
- Launches multiple processes (Process-1, Process-2)  
- Logs events to `system_log.txt`  
- Simulates:
  - System Boot  
  - Individual process start & termination  
  - System Shutdown  

Shows how real operating systems handle concurrent processes.

---

## 📌 Task 3 — Inter-Process Communication (IPC using Pipes)

**File:** `task3.py`

Implements IPC using:
- `os.pipe()` → creates a unidirectional communication channel  
- `os.fork()` → parent and child processes  

Behavior:
- Parent sends a message through the pipe  
- Child receives and prints it  

⚠️ **Note:** This program works only on **Linux / Unix** because `fork()` is not available on Windows.

---

## 📌 Task 4 — Virtual Machine Detection

**File:** `task4.py`

This task demonstrates:
- Checking system information using Linux commands (`uname`, `lscpu`)  
- Detecting whether the system is running on a Virtual Machine using Python (`systemd-detect-virt`)  
- Prints either “Real hardware” or the type of virtual environment detected  

---

## 📌 Task 5 — CPU Scheduling Algorithms

**File:** `task5.py`

Implements common scheduling algorithms:
- FCFS (First Come First Serve)  
- SJF (Shortest Job First)  
- Round Robin (with time quantum)  
- Priority Scheduling  

Displays for each algorithm:
- Burst Time (BT)  
- Waiting Time (WT)  
- Turnaround Time (TAT)  

---

## 🚀 How to Run

Run any task using the format:

```
python taskX.py
```

Example:

```
python task1.py
```
