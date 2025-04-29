# Web Google Network Analysis

This project analyzes the web graph from Google, visualizing and exploring its network properties using NetworkX and other Python libraries.

## Dataset

The dataset used in this project is the Web Graph from Google, which was released in 2002. It was collected by the [Stanford Network Analysis Project (SNAP)](https://snap.stanford.edu/data/web-Google.html) and represents a portion of the web graph where nodes represent web pages and directed edges represent hyperlinks between them.

### Dataset Statistics

| Metric | Value |
|--------|-------|
| Nodes | 875,713 |
| Edges | 5,105,039 |
| Nodes in largest WCC | 855,802 (0.977) |
| Edges in largest WCC | 5,066,842 (0.993) |
| Nodes in largest SCC | 434,818 (0.497) |
| Edges in largest SCC | 3,419,124 (0.670) |
| Average clustering coefficient | 0.5143 |
| Number of triangles | 13,391,903 |
| Fraction of closed triangles | 0.01911 |
| Diameter (longest shortest path) | 21 |
| 90-percentile effective diameter | 8.1 |

## Getting Started

### Prerequisites

- Python 3.x
- Jupyter Notebook
- Required Python packages: networkx, matplotlib, numpy, pandas, seaborn, powerlaw, etc.

### Setup Instructions

1. Clone this repository:
   ```
   git clone https://github.com/batuhannoz/web-google-network-analyze.git
   cd web-google-network-analyze
   ```

2. Extract the data from the compressed file:
   ```
   gunzip web-Google.txt.gz
   ```
   This will create the `web-Google.txt` file needed for analysis.


3. Run Jupyter Notebook:
   ```
   jupyter notebook
   ```

4. Open the `web-google-analyze.ipynb` notebook file in your browser.

## Features

The Jupyter notebook includes various network analyses:

- Basic network statistics (nodes, edges, degree distribution)
- Connectivity analysis (components, diameter, path length)
- Power law analysis of degree distributions
- Centrality measures (PageRank, betweenness, closeness)
- Clustering coefficient analysis
- Community detection
- k-core decomposition

## Visualization

After running the analysis, the network is exported in GEXF format, which can be opened with network visualization tools like [Gephi](https://gephi.org/).

Two files are generated:
- `web_google_sample.gexf`: A smaller sample of the network that can be easily opened in Gephi
- `web_google_full.gexf`: The complete network (note: this file is very large and may be difficult to open without significant computing resources)

It's recommended to use the sample version for visualization as the full version is extremely large and requires substantial computational resources to visualize effectively.

- Düzce üniversitesi - Bilgisayar Mühendisliği - BM479 Kompleks Ağ Analizi - Dr. Öğr. Üyesi Sultan Zavrak - Bahar, 2024/2025