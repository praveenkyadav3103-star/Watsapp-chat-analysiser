# Watsapp-chat-analysiser
# GroupDNA — WhatsApp Group Behaviour Analyzer

A Python and NumPy-based tool that analyzes WhatsApp group-chat data to identify activity patterns, response behaviour, frequently used words, silent streaks, and participant personality archetypes.

##  Project Overview

| Project Detail | Information |
| --- | --- |
| **Project Title** | CSE 2026 — Code, Canteen & Chaos |
| **Developed by** | Praveen Kumar Yadav |
| **Batch** | Data Analytics |
| **Project Type** | Data Analytics Minor Project |
| **Technologies Used** | Python, NumPy, File I/O, and Datetime |
| **Dataset** | Synthetic Indian College WhatsApp Group Chat (`cse_2026_survival_squad_10_members.txt`) |
| **Submitted To** | Adyapan Academy |
| **Submission Date** | August 2026 |

##  Project Constraints

The project was intentionally developed using Python fundamentals without relying on high-level data libraries:

### Allowed
* Python fundamentals
* Strings and string methods
* Lists and dictionaries
* Loops and conditional statements
* Functions
* File I/O
* NumPy
* Datetime

### Not Used
* Pandas, Matplotlib, Seaborn, Plotly
* Regular expressions
* `collections.Counter`, `collections.defaultdict`
* NLTK, Scikit-learn
* Pre-built WhatsApp-analysis libraries

##  Seven-Day Build Log

| Day | Work Completed |
|---|---|
| Day 1 | Dataset reading and chat-parser development |
| Day 2 | Group overview and participant statistics |
| Day 3 | Word-frequency analysis and Top Words |
| Day 4 | NumPy activity matrix and text-based heatmap |
| Day 5 | Response-time and silent-streak analysis |
| Day 6 | Personality-archetype detection |
| Day 7 | Final report, testing and documentation |

##  How to Run the Project

1. Open `GroupDNA_PRAVEEN.ipynb` in Google Colab or Jupyter Notebook.
2. Run the library-import cell.
3. Upload `cse_2026_survival_squad_10_members.txt` when prompted.
4. Run all cells sequentially from top to bottom.
5. View the complete GroupDNA report at the end of the notebook.

graph TD
    %% Styling / Colors
    classDef inputStyle fill:#e1f5fe,stroke:#01579b,stroke-width:2px;
    classDef processStyle fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px;
    classDef outputStyle fill:#fff3e0,stroke:#e65100,stroke-width:2px;

    %% Nodes
    A["Raw WhatsApp Export <br/> (cse_2026_survival_squad_10_members.txt)"]:::inputStyle --> B["Feature 1: Chat Parser <br/> • Line Filtering & Cleaning <br/> • Multi-line & System Msg Handling"]:::processStyle
    
    B --> C["Parsed Message List <br/> (Timestamps, Senders, Text)"]:::processStyle

    C --> D1["Feature 2: Group Overview <br/> • Active/Inactive Leaders <br/> • Per-Person Stats"]:::processStyle
    C --> D2["Feature 3: Temporal Trends <br/> • Busiest Days & Peak Hours"]:::processStyle
    C --> D3["Feature 4: NumPy Matrix <br/> • 10x24 Activity Heatmap"]:::processStyle
    C --> D4["Feature 5: Word Frequency <br/> • Stop-word Removal & Top Words"]:::processStyle
    C --> D5["Feature 6: Response & Streaks <br/> • Gap Calculation & Silent Days"]:::processStyle
    C --> D6["Feature 7: Archetype Detection <br/> • Rule-Based Persona Matching"]:::processStyle

    D1 --> E["Feature 8: Final GroupDNA Report <br/> • Comprehensive Text Summary"]:::outputStyle
    D2 --> E
    D3 --> E
    D4 --> E
    D5 --> E
    D6 --> E

    E --> F["Project Deliverables <br/> • Console Output / Summary <br/> • Documentation & README"]:::outputStyle

##  Repository Files

```text
GroupDNA-WhatsApp-Chat-Analyzer/
│
├── GroupDNA_PRAVEEN.ipynb
├── cse_2026_survival_squad_10_members.txt
└── README.md
