# DFA English Word Recognizer

## 📌 Project Overview
This project implements a **Deterministic Finite Automaton (DFA)** to recognize specific English words from input text. The system processes text character by character (left to right) and identifies predefined keywords such as conjunctions, adverbs, and adjectives.

It also provides word detection, position tracking, DFA visualization, and detailed reporting.

---

## 🎯 Recognized Keywords
The DFA recognizes the following words:

- and  
- most  
- good  
- bad  
- pretty  
- dirty  
- blue  

---

## ⚙️ Features
- DFA-based string processing (state machine simulation)
- Character-by-character input scanning
- Word boundary validation
- Accept / Reject classification
- Keyword occurrence tracking
- Position indexing of matched words
- Snippet highlighting in results
- DFA diagram generation using Graphviz
- Automatic report generation

---

## 🧠 How It Works
1. Input text is converted to lowercase for consistency  
2. DFA starts at initial state (q0)  
3. Each character is processed sequentially  
4. State transitions follow predefined DFA rules  
5. If a final state is reached → keyword is accepted  
6. Invalid transitions move the system to a trap state  
7. Word boundary checks ensure correct word detection  

---

## 🛠️ Tech Stack
- Python 🐍  
- Graphviz (for DFA visualization)  
- Pillow (image rendering support)  
- Tkinter (optional GUI interface)

---

## 📂 Project Structure
```text
CPT411_ASSIGNMENT1/
│
├── diagrams/                 # Generated DFA diagrams
├── output reports/           # Output result files
├── text files/               # Input test datasets
├── src/L5_English_Conjunctions_Adverb_Adjectives_Finder.py
└── README.md
```
---

## 📊 Output Example
**Accepted Case**
- Keyword detected in text
- Positions recorded
- Snippet displayed with highlighted word
- Status: ACCEPTED

**Rejected Case**
- No keyword found in input text
- Status: REJECTED

---

## 📈 DFA Visualization

Each keyword has its own DFA representation generated using Graphviz.

Structure includes:

- q0 → initial state
- q1, q2, ... → transition states
- q_accept → final accepting state
- trap → invalid state for rejection

---

## 🚀 How to Run
```bash
python L5_English_Conjunctions_Adverb_Adjectives_Finder.py
```

Install dependencies:

```bash
pip install graphviz pillow
```

Graphviz setup:

Download and install from:
https://graphviz.org/download/

Ensure Graphviz is added to system PATH.

---

## 📌 Key Learning Outcomes
- Understanding Deterministic Finite Automata (DFA)
- Text processing using state machines
- Pattern recognition in strings
- Visualization of automata using Graphviz
- Practical implementation of formal language theory

---
  
