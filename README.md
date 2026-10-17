# FuzzyNote AI 📚

**A lightweight, typo-tolerant note retrieval system built with Python and RapidFuzz.**

FuzzyNote AI helps users find relevant notes even when their search queries contain spelling mistakes, abbreviations, or incomplete keywords.

Instead of relying only on exact text matches, the system compares queries against stored note titles, content, and aliases, then ranks matching notes by string similarity.

## ✨ Features

- **Fuzzy search:** Handles approximate spelling and wording.
- **Alias matching:** Supports shortcuts such as `ML` and `DBMS`.
- **Query normalization:** Handles capitalization and extra whitespace.
- **Ranked results:** Displays higher-scoring matches first.
- **Threshold filtering:** Hides results below a configurable similarity score.
- **Top-result limit:** Returns a manageable list of relevant notes.
- **Interactive search:** Lets users perform multiple searches in one session.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Application logic |
| RapidFuzz | String similarity and fuzzy matching |
| Dictionaries | Store note titles, content, and aliases |

## 🧠 How It Works

1. The user enters a search query.
2. The system normalizes the query.
3. Exact title and alias matches are checked.
4. The query is compared with stored note information using fuzzy string similarity.
5. Results are filtered and sorted by score.
6. The highest-ranked matches are displayed.

## 📂 Project Structure

```text
noteforge-search/
├── main.py
├── requirements.txt
├── README.md
├── Smart_Notes_Finder.ipynb
└── Smart_Notes_Finder_final.ipynb
```

The Python script is the main application. The notebooks can be retained as development and experimentation records.

## 🚀 Getting Started

### Prerequisites

- Python 3.9 or newer
- pip

### Installation

Clone the repository:

```bash
git clone https://github.com/MithravindaU/noteforge-search.git
```

Enter the project directory:

```bash
cd noteforge-search
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python main.py
```

## 💡 Example Searches

| Query | Intended behaviour |
|---|---|
| `ml` | Finds the Machine Learning alias |
| `machin learnng` | Attempts to match a misspelled query |
| `database` | Finds notes related to database systems |
| `sorting` | Finds notes related to sorting algorithms |
| `unrelated topic` | May return no results if nothing meets the threshold |

Actual results depend on the stored note content and similarity scores.

## 📖 Core Concepts Demonstrated

- Fuzzy string matching
- Information retrieval fundamentals
- Query normalization
- Alias-based lookup
- Similarity scoring and ranking
- Threshold-based filtering
- Basic Python data structures

## ⚠️ Current Limitations

- Notes are stored in the source code rather than a persistent database.
- The application uses predefined sample notes.
- Fuzzy similarity does not understand meaning in the same way a semantic embedding model can.
- Similarity scores are not calibrated confidence probabilities.
- Search quality depends on the note content, aliases, and selected threshold.

## 🔮 Future Improvements

- Import notes from text and PDF files.
- Add persistent storage so users can create and edit notes.
- Build a simple web interface.
- Add automated tests for typos, aliases, empty queries, and unrelated searches.
- Compare fuzzy matching with TF-IDF and semantic search.
- Evaluate retrieval quality using a small, documented test dataset.

## 🎯 Project Goal

FuzzyNote AI explores how lightweight retrieval techniques can make searching stored information more forgiving and user-friendly. It serves as a foundation for learning about search engines, query processing, and information retrieval.

## 👩‍💻 Author

**Mithravinda U**

GitHub: [@MithravindaU](https://github.com/MithravindaU)

---

*Built as a learning project exploring Python and intelligent search techniques.*
