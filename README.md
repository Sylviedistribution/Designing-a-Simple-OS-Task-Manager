# 📘 Operating System Task Management Simulation


## 📌 Project Overview

This project simulates core concepts of Operating Systems through four major components:

CPU Scheduling Algorithms (FCFS & Round Robin)
Process Synchronization (Mutex-based solution)
Memory Management (FIFO & LRU Page Replacement)
Disk Scheduling (FCFS & SSTF)

The objective is to analyze how different algorithms impact system performance in terms of efficiency, fairness, and resource utilization.

### ⚙️ Part 1: CPU Scheduling

Algorithms Implemented:
-First Come First Served (FCFS)
-Round Robin (Quantum = 2)

Key Metrics
Waiting Time
Completion Time
Average Waiting Time
Key Observation

Round Robin improves responsiveness and fairness by sharing CPU time between processes, while FCFS is simpler but can delay short processes.

### 🔐 Part 2: Process Synchronization

Problem

Two processes increment a shared variable (counter). Without synchronization, race conditions occur, leading to incorrect final values.

Solution

A Mutex lock is used to ensure mutual exclusion during updates.

Result

This guarantees data consistency and prevents concurrent access issues.

### 🧠 Part 3: Memory Management

Page Replacement Algorithms
FIFO (First In First Out)
LRU (Least Recently Used)
Page Reference String

1, 2, 3, 2, 4, 1, 5

Key Observation

LRU performs better than FIFO because it considers recent usage patterns, reducing page faults.

### 💽 Part 4: Disk Scheduling

Algorithms Implemented
FCFS (First Come First Served)
SSTF (Shortest Seek Time First)
Key Observation

SSTF significantly reduces total head movement compared to FCFS, improving disk efficiency. However, it may cause starvation for distant requests.

### 📊 Summary of Results

| Component        | Better Algorithm | Reason                     |
|------------------|------------------|----------------------------|
| CPU Scheduling   | Round Robin      | Better responsiveness      |
| Memory Management| LRU              | Fewer page faults          |
| Disk Scheduling  | SSTF             | Lower head movement        |
| Synchronization  | Mutex            | Prevents race conditions   |

### 🎯 Conclusion

This simulation highlights the trade-offs in Operating System design. There is no universally optimal algorithm; each approach balances performance, fairness, and complexity differently depending on system requirements.

📁 Technologies / Concepts Used
CPU Scheduling Algorithms
Process Synchronization
Memory Paging
Disk Scheduling Algorithms
🚀 Learning Outcome

This project improves understanding of:

How operating systems manage processes
How resources are allocated efficiently
Why synchronization is critical in concurrent systems