# Graph-Theory-Project-Path-Analysis-in-E-Commerce-Navigation
Graph‑Theory course project that models user‐navigation data as a directed graph and applies shortest‑path and frequency analysis to uncover the most valuable purchase funnels.

## Project Overview
1. Load click‑stream data (navigation_data.csv).
2. Build a directed graph where each edge represents a user moving from one page to the next.
3. Analyze
4. Global shortest paths between all pairs.
5. Top‑5 most frequent navigation edges.
6. Evaluate model accuracy on a 20 % hold‑out sample (precision / recall / F1).
7. Visualize the navigation graph with NetworkX + Matplotlib.

## Requirements
- Python 3.8+
- pandas 2.x
- networkx 3.x
- matplotlib 3.x

### Install everything in one line:
pip install pandas networkx matplotlib

## Usage
python path_analysis.py            # Assumes navigation_data.csv in same folder
python path_analysis.py --file ~/data/nav_data.csv

## How It Works
1.  load_dataset()	Read CSV into a DataFrame.
2.	preprocess_data()	Convert consecutive pages into (source, dest) edges.
3.	build_graph()	Create a nx.DiGraph from the edge list.
4.	analyze_paths()	Compute all‑pairs shortest paths & count edge frequency.
5.	evaluate_graph()	Compare graph edges against a test split (precision / recall / F1).
6.	visualize_graph()	Render nodes, edges, and labels with Matplotlib.

## Acknowledgements
- NetworkX for graph algorithms
- Matplotlib for visualization
- Pandas for data wrangling
