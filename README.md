# File-Recovery-And-Optimization-Tool
File Recovery and Optimization Tool
  Project Overview
  
  File Recovery and Optimization Tool is a C++ based system utility that safely optimizes file storage by moving selected files into a secure      vault instead of permanently deleting them. The tool supports undo and redo operations, allowing users to recover or re-delete files easily.
    
  This project demonstrates Operating System concepts, file system management, and data structures like stack and queue.
  
  Objectives
    Safely remove unwanted files without permanent deletion
    Allow file recovery using undo functionality
    Re-delete files using redo functionality
    Demonstrate OS concepts such as file systems, paging, and virtual memory
    Apply data structures in a real-world scenario
  
  🛠️ Technologies Used

  Language: C++
  Libraries:
    <filesystem>
    <queue>
    <stack>
    <vector>
    
  Compiler: GCC / Clang (C++17 or later)
  
  🧠 Concepts Used
  Operating System Concepts
    File System Management
    Safe File Deletion (Move instead of Delete)
    Virtual Memory
    Paging
    System Calls
    Memory Management
  
  Data Structures
    Queue → Breadth First Search (Directory Traversal)
    Stack → Undo / Redo Operations
    Vector → File Storage
  
  How It Works
    User provides a directory path
    The program scans directories using BFS (Queue)
    All files are listed
    User selects a file to optimize (safe delete)
    File is moved to a vault folder
    Undo operation restores the file
    Redo operation deletes it again
  
  Undo/Redo Mechanism
    Undo Stack: Stores deleted file operations
    Redo Stack: Stores recovered file operations
    Both operations run in O(1) time
