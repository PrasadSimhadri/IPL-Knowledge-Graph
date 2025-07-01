# 🏏 IPL Knowledge Graph

This project visualizes IPL match data as an interactive **Knowledge Graph** using Python, NetworkX, and Matplotlib. Each player is represented with their team as a combined node (e.g. `Virat Kohli (RCB)`), and edges represent meaningful relationships like matches played, opponents faced, venues hosted, and match results.

---

## 📘 Features

- 🔄 **Directional edges** showing relations like:
  - `playedInMatch`
  - `playedAgainst`
  - `wonMatch`
  - `heldAt`
- 🎨 **Role-based coloring**: Batsman, Bowler, All-rounder, Wicket-Keeper
- 📊 **Edge weight** proportional to runs scored
- 🧠 Built from a structured IPL CSV dataset

---

## 📁 Project Structure

```

ipl-knowledge-graph/
├── data/
│   └── ipl\_matches.csv         # Enriched IPL dataset
├── ipl\_knowledge\_graph.ipynb   # Jupyter Notebook
└── README.md                   

````

---

## 🛠️ Getting Started

### ✅ Prerequisites

Make sure you have:

- Python 3.8+
- Jupyter Notebook or any Python IDE

### 🔧 Installation

Clone the repo and install dependencies:

```bash
git clone https://github.com/PrasadSimhadri/IPL-Knowledge-Graph.git
cd ipl-knowledge-graph
````

Or manually install:

```bash
pip install pandas networkx matplotlib
```

---

## 🚀 Usage

1. Open the notebook:

   ```bash
   jupyter notebook ipl_knowledge_graph.ipynb
   ```
2. Run all cells to:

   * Load dataset
   * Build the graph
   * Visualize the IPL knowledge network

---

## 📌 Dataset Columns

| Column        | Description                         |
| ------------- | ----------------------------------- |
| `Player`      | Player name                         |
| `Team`        | Player's team                       |
| `Opponent`    | Opposing team                       |
| `Match`       | Match ID or name                    |
| `Venue`       | Stadium/City where match was held   |
| `MatchResult` | Whether the player's team won       |
| `Runs`        | Runs scored by player in that match |
| `Role`        | Player type (Batsman, Bowler, etc.) |

---

## 🙌 Acknowledgements

This project was built for educational purposes to demonstrate how structured tabular data can be converted into a semantic graph.

---
