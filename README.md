# NITCbase

A modular RDBMS implementation in C++ for educational purposes.

## 📖 Overview

NITCbase is a teaching-focused relational database management system designed to help students understand RDBMS internals by building one layer-by-layer. Implemented in C++ for Unix/Linux systems, it features:

- 8 architectural layers from physical storage to SQL-like interface
- Core RDBMS components including buffer management and B+ tree indexing
- Two CLI interfaces for database operations and disk management

## 🏗 Architecture Layers

1. **Physical Layer**: Disk I/O operations
2. **Buffer Layer**: LRU-based cache management
3. **B+ Tree Layer**: Index implementation
4. **Block Access Layer**: DML operations
5. **Cache Layer**: Relation/attribute caching
6. **Algebra Layer**: SELECT, PROJECT, JOIN
7. **Schema Layer**: CREATE, DROP, ALTER
8. **Frontend Layer**: SQL-like CLI

## ✨ Key Features

- SQL-like query interface
- Table operations (create/drop/alter)
- CRUD operations with indexing
- Modular, education-focused design
- Guided implementation approach

## 🛠 Tech Stack

- **Language**: C++17
- **Platform**: Linux/Unix
- **Interfaces**: Custom CLI and XFS shell


## 🚀 Quick Start

### Prerequisites
- Linux/Unix OS
- g++ compiler
- Basic RDBMS knowledge

### Compilation
```bash
g++ -std=c++17 -o nitcbase main.cpp Disk.cpp StaticBuffer.cpp ...
