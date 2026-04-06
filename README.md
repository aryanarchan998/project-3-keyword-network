# Project 3: Exploring Keyword Co-occurrence Networks in Scientific Publications

## Overview 
This project analyzes keyword co-occurrence patterns in scientific publications using Python. The dataset contains article titles and up to 13 keywords per article. By analyzing how frequently keywords appear together, we construct a weighted network that reveals relationships between research topics and identifies the most central concepts.

## Objectives 
The main objectives of this project are: 
- Transform keyword data into a network structure using an adjacency matrix 
- Build and analyze a weighted keyword network 
- Compute key network metrics such as degree and strength
- Identify the most important keywords and keyword pairs 
- Visualize relationships between degree and strength 


---

## Files in this Repository
- `notebook.ipynb` - Jupyter/Colab notebook with all code, outputs, and explanations
- `report.md` - short written report interpreting the results
- `data/keywords_data.csv` - dataset used for the project

## Dataset
The dataset used in this project contains academic publication data. Each row represents a single article and includes:

- One title column  
- Up to 12 keyword columns  

## Tools Used
- Python
- pandas
- networkx
- matplotlib
- Google Colab


## Methodology

### 1. Data Preparation 
- Extracted only keyword columns from the dataset 
- Converted all keywords to lowercase 
- Removed rows with no keyword data 

### 2. Adjacency Matrix Construction 
- Built a symmetric weighted adjacency matrix 
- Rows and columns represent unique keywords 
- Each cell counts how often two keywords appear together 


### 3. Network Construction 
- Converted the adjacency matrix into a weighted graph using NetworkX  
- Nodes represent keywords  
- Edges represent co-occurrence relationships  
- Edge weights indicate frequency of co-occurrence


### 4. Network Metrics 

- Degree: Number of unique keywords a keyword connects 
- Strength: Total sum of co-occurrence weights 

### 5. Analysis 
- Identified top 10 keywords by degree 
- Identified top 10 keywords by strength 
- Identified top 10 keyword pairs by weight 

### 6. Visualization 
- Created a scatter plot of degree (x-axis) vs strength (y-axis)  
- Used matplotlib for visualization

##Key Findings 
- Organizational behavior is the most central keyword, with the highest degree and strength
- Strong keyword pairs (e.g., organizational behavior and organizational effectiveness) indicate common research themes  
- The scatter plot shows a positive relationship between degree and strength, meaning highly connected keywords also tend to co-occur more frequently  

