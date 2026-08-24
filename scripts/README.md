# GridCare: Energy Grid Data Analysis & Network Modeling

## Project Overview

GridCare is data science project focused on analyzing electricity grid infrastructure through data engineering, exploratory data analysis, visualization, and network modeling.

The project works with utility, substation, and transmission-line datasets to explore patterns within energy infrastructure and represent relationships between grid components as a network.

The project demonstrates how data analysis and network science can be applied to understand complex infrastructure systems and support data-driven decision-making.


## Objectives

The main objectives of the project were to:

- Clean and prepare energy infrastructure datasets for analysis.
- Explore patterns in electricity infrastructure using statistical analysis and visualization.
- Analyze voltage levels, capacity, line types, and commissioning years.
- Integrate utility, substation, and transmission-line datasets.
- Model the electricity grid as a network using NetworkX.
- Visualize relationships between grid components.
- Identify patterns that could support further analysis of energy infrastructure.


## Dataset

The project uses three main datasets:

### Utilities

Contains information about electricity utility infrastructure and associated characteristics.

### Substations

Contains information about substations, including attributes such as:

- Name
- Region
- Voltage
- Capacity
- Coordinates

### Transmission Lines

Contains information about connections between grid components, including:

- Length
- Voltage
- Capacity
- Status
- Type

These datasets were cleaned and integrated to create a more comprehensive representation of the electricity grid.


## Data Engineering and Cleaning

The data preparation process included:

- Inspecting datasets using `head()` and `tail()`.
- Examining data types and structure using `info()`.
- Generating descriptive statistics using `describe()`.
- Checking for missing values using `isnull().sum()`.
- Checking dataset dimensions using `shape`.
- Cleaning and preparing the datasets for analysis.
- Joining relevant datasets.
- Creating processed data for subsequent analysis.

The cleaned datasets were then used for exploratory analysis and network modeling.

---

## Exploratory Data Analysis

The project used exploratory data analysis to identify patterns and characteristics within the energy infrastructure.


## Network Modeling

The electricity grid was modeled as a graph using **NetworkX**.

```python
G = nx.Graph()

In the network model:

Nodes represent grid infrastructure components.
Edges represent connections between those components

The network was visualized using a spring layout:

pos = nx.spring_layout(G, seed=42)

## Technologies Used

- Python
- Pandas
- Matplotlib
- NetworkX
- Jupyter Notebook
- Git
- GitHub

## Project Structure
gridcare-energy-grid-analysis/
│
├── data/
│   ├── lines.csv
│   ├── substations.csv
│   └── utilities.csv
│
├── notebooks/
│   ├── Data_Engineering.ipynb
│   ├── exploratory_analysis.ipynb
│   ├── network_graph.ipynb
│   └── processed_data.csv
│
├── scripts/
│   └── generate_grid_data.py
│
└── README.md


## Future Work

Future improvements could include:

- Calculating network centrality measures.
- Identifying critical substations and transmission links.
- Developing interactive maps of the electricity grid.
- Applying machine learning to infrastructure risk or demand prediction.
