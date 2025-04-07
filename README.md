NITCbase
A Relational Database Management System (RDBMS) Implementation Project
📘 Introduction
NITCbase is an academic RDBMS implementation project aimed at helping undergraduate students understand the architecture and data structures behind relational databases by building one from scratch using C++ on a Unix/Linux environment.

This system is built in eight modular layers, starting from low-level disk operations up to a fully functional SQL-like frontend interface. Through this project, students gain hands-on experience with key database components like buffer management, B+ trees, query execution, and schema management.

🏗️ Architecture
NITCbase is designed in 8 layers:

Physical Layer – Low-level disk read/write (given)

Buffer Layer – Disk buffer management (LRU replacement)

B+ Tree Layer – Indexing with B+ trees

Block Access Layer – Implementation of core DML operations

Cache Layer – In-memory relation and attribute caches

Algebra Layer – SQL-like DML support: SELECT, PROJECT, JOIN

Schema Layer – DDL support: CREATE, DROP, ALTER

Frontend Layer – CLI support for SQL-like queries

The project includes two command-line interfaces:

Frontend Interface: For SQL-like interactions

XFS Interface: For disk and file system operations

✨ Features
SQL-like query support:

CREATE, DROP, ALTER tables

INSERT, SELECT, PROJECT, JOIN

B+ tree indexing (CREATE INDEX, DROP INDEX)

Disk-level operations via XFS Interface

Modular, layered architecture

Clean abstraction and separation of concerns

Fully guided implementation roadmap

🧰 Tech Stack
Language: C++

Platform: Linux/Unix

CLI Interfaces: Custom-built Frontend & XFS Shell

📂 Project Structure
graphql
Copy
Edit
NITCbase/
├── Disk.cpp               # Physical disk access (given)
├── StaticBuffer.cpp       # Buffer Layer
├── BPlusTree.cpp          # B+ Tree Layer
├── BlockAccess.cpp        # Block Access Layer
├── OpenRelTable.cpp       # Cache Layer
├── Schema.cpp             # Schema Layer
├── Algebra.cpp            # Algebra Layer
├── FrontendInterface.cpp  # Frontend UI (given)
├── Frontend.cpp           # Frontend Programming Interface (partially given)
├── Documentation/         # Specs, design docs, tutorials
└── Roadmap.md             # Guided implementation stages
🚀 Getting Started
Prerequisites
A Unix/Linux system

C++ compiler (e.g. g++)

Basic familiarity with RDBMS concepts and data structures

Compilation
Compile the project using g++. Example:

bash
Copy
Edit
g++ -std=c++17 -o nitcbase main.cpp Disk.cpp StaticBuffer.cpp ...
You can compile modules incrementally as you progress through the roadmap.

📚 Documentation
You are provided with:

A full implementation of:

Disk.cpp (physical layer)

XFS Interface

Frontend Interface

Class stubs and algorithm specifications for each layer

Tutorials and in-depth guides for complex parts (e.g., B+ trees)

A detailed implementation roadmap guiding you step by step

🧑‍🏫 For Instructors
This project is structured to maximize pedagogical value. Students gradually build up each layer, integrating both theoretical understanding and practical coding skills.

Emphasizes modular understanding

Encourages clean abstractions

Involves ~3000 lines of C++ code upon completion

📌 Notes
The system currently does not support concurrency

The final RDBMS will be able to handle a range of SQL-like operations on a simulated disk system

Focus is placed on clarity, structure, and educational value over real-world optimization

🎓 Credits
Developed as part of the undergraduate curriculum at NIT Calicut for educational purposes.
