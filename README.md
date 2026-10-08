# 🎮 Gamified Feedback Analyzer — Data Structures & Algorithms (DSA) Engine

<div align="center">

[![C++](https://img.shields.io/badge/Language-C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)](https://isocpp.org/)
[![DSA](https://img.shields.io/badge/Algorithms-Max--Heap%20%7C%20Hash%20Maps%20%7C%20Stacks-orange?style=for-the-badge)](#-data-structures--complexity)
[![Architecture](https://img.shields.io/badge/Paradigm-Gamified%20NLP%20Analytics-green?style=for-the-badge)](#-core-features)
[![Platform](https://img.shields.io/badge/Platform-Windows%20Console-0078D6?style=for-the-badge&logo=windows&logoColor=white)](#-build--execution)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

<br />

**An algorithmic feedback sentiment classification and gamification engine.**  
*Harnessing fundamental Data Structures (Linked Lists, Hash Maps, Priority Queues / Max-Heaps, and LIFO Stacks) to deliver real-time user scoring, undo tracking, and dynamic leaderboards.*

[**Explore Code (`src/`) →**](src/feedback_analyzer.cpp) • [**View Technical Report (`docs/`) →**](docs/dsa_feedback_analyzer_report.docx)

</div>

---

## 📌 Executive Summary

The **Gamified Feedback Analyzer** transforms unstructured user input (suggestions, complaints, appreciations) into actionable organizational insights. Developed as an advanced **Data Structures & Algorithms** project, it replaces naive linear searching with optimized standard library containers and bespoke pointer-based structures, incentivizing user engagement through dynamic scoring algorithms, trivia challenges, and level progression badges.

---

## 🧩 Data Structures & Complexity

| Data Structure | Implementation | Applied Component | Time Complexity |
| :--- | :--- | :--- | :--- |
| **Doubly/Singly Linked List** | `struct Feedback* next` | Sequential feedback history per user | $O(1)$ Insertion |
| **Associative Hash Map** | `std::map<string, Feedback*>` | Instant retrieval of feedback by username | $O(\log N)$ Lookup |
| **Max-Heap (Priority Queue)** | `std::priority_queue<pair<int, string>>` | Dynamic competitive leaderboard sorting | $O(\log N)$ Insert / $O(1)$ Top |
| **LIFO Stack** | `std::stack<Feedback*>` | Rollback & Undo operations | $O(1)$ Push / Pop |

---

## ✨ Core Features

* 📊 **Categorization Engine**: Automated classification across Suggestions, Complaints, and Appreciations.
* 🏆 **Gamified Scoring Model**: Point weighting calculated based on submission substance, length, and sentiment category.
* 🥇 **Real-Time Leaderboard**: Live ranking generated on-the-fly using binary heap structures (`priority_queue`).
* ↩️ **Atomic Undo Stack**: Undo accidental submissions or reviews with state reversion.
* 🧠 **Trivia & Engagement Loops**: Integrated engineering trivia and productivity micro-quizzes.
* 💾 **Disk Persistence**: Disk state logging and persistence across user sessions.

---

## 📂 Project Structure

```text
gamified-feedback-analyzer-dsa/
├── docs/
│   └── dsa_feedback_analyzer_report.docx  # Detailed algorithmic & design report
├── src/
│   └── feedback_analyzer.cpp              # Core C++ DSA implementation
├── .gitignore                             # Ignore rules for compiled binaries & logs
└── README.md                              # Portfolio case study & documentation
```

---

## 🚀 Build & Execution

### Prerequisites
* GCC / G++ (MinGW on Windows) or MSVC Compiler

### Compilation
```bash
# Clone the repository
git clone https://github.com/lizzz-dev/gamified-feedback-analyzer-dsa.git
cd gamified-feedback-analyzer-dsa

# Compile
g++ -std=c++17 -O2 src/feedback_analyzer.cpp -o FeedbackAnalyzer.exe

# Execute
./FeedbackAnalyzer.exe
```

---

## 👩‍💻 Author

**Leeza Nawaz**  
*Creative Frontend & AI/Software Engineer*  
* **GitHub**: [@lizzz-dev](https://github.com/lizzz-dev)  
* **Repository**: [lizzz-dev/gamified-feedback-analyzer-dsa](https://github.com/lizzz-dev/gamified-feedback-analyzer-dsa)
