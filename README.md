🗓️ Conference Scheduling
A Python-based solution for solving the Conference Scheduling Problem (CSP) using a Constraint Satisfaction Problem (CSP) approach. This project assigns papers to appropriate sessions in a conference schedule while satisfying multiple constraints.

📌 Table of Contents
About the Project

Features

Technologies Used

Problem Description

Installation

Usage

Folder Structure

License

📖 About the Project
The goal of this project is to optimally schedule a set of research papers into conference sessions while respecting a number of hard and soft constraints. It uses a CSP (Constraint Satisfaction Problem) formulation with backtracking search, MRV (Minimum Remaining Values), and LCV (Least Constraining Value) heuristics to find valid solutions.

This project was part of the AI course at Sharif University of Technology.

✨ Features
CSP formulation of the scheduling problem

Backtracking search with MRV & LCV heuristics

Flexible constraint handling:

No overlapping of papers

Author time availability

Topic similarity within sessions

Limited number of papers per session

CSV input/output for easy integration

🛠 Technologies Used
Python 3

NumPy

Pandas

CSV

📚 Problem Description
Given:

A list of papers

A number of sessions

Author availability times

Paper topic similarities

Find a valid assignment of papers to sessions such that:

No author is scheduled for two presentations at the same time

Papers in the same session are topically coherent

No session exceeds its capacity

Each paper is scheduled exactly once

🚀 Installation
Clone the repository:

bash
Copy
Edit
git clone https://github.com/yasserzs3/Conference-Scheduling.git
cd Conference-Scheduling
Install the required dependencies:

bash
Copy
Edit
pip install -r requirements.txt
▶️ Usage
Place your input CSV files (authors, papers, sessions) in the input/ directory.

Run the main script:

bash
Copy
Edit
python main.py
The scheduled sessions will be written to the output/ directory.

You can modify the number of sessions or papers per session by editing the configuration in the main script.

🗂 Folder Structure
graphql
Copy
Edit
Conference-Scheduling/
│
├── input/                   # Input CSV files (papers, authors, availability)
├── output/                  # Generated schedule output
├── csp/                     # CSP logic and problem formulation
│   ├── constraints.py
│   ├── csp.py
│   └── backtracking.py
│
├── utils/                   # Utility functions for preprocessing and I/O
│   ├── paper_reader.py
│   ├── availability_reader.py
│   └── similarity_calculator.py
│
├── main.py                  # Entry point of the application
└── README.md
📄 License
This project is licensed under the MIT License. See the LICENSE file for more details.

