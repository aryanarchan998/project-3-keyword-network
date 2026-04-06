# Project 3 Report: Keyword Co-occurrence Network Analysis 

## Introduction 

This project explores keyword co-occurrence patterns in scientific publications using network analysis. The objective of this project is to understand how different research topics are connected by analyzing how often keywords appear together in the same articles. We will be transforming keyword data into a weighted network and will be identifying central themes, concepts and strong relationships between topics.  

---

## Methodology 

The dataset used in this project consists of academic articles, each containing up to 12 keywords. First step was to extract only the keyword columns and converting all keywords to lowercase. The rows that had no keyword data were removed to ensure meaningful analysis. 

The next task was to construct a weighted adjacency matrix. In the matrix both rows and columns represent unique keywords, and each cell records how many times two keywords appear together in the same article. The matrix is symmetrical because the co-occurrence relationships go both ways (bi-directional).

Now the adjacency matrix was then converted into a weighted network using network. The nodes represent keywords, edges represent the relationship and the edge weights represent how frequently two keyword appear together. The main two key metrics degree and strength were calculated. The degree being the number of unique keywords connected to a keyword and the strength being total weight of all connections for a keyword. 


## Results and Analysis 

The analysis showcased that certain keywords are significantly more central and active than others. Particularly "organizational behavior" came out as the most important keyword revealing to have the highest degree and highest strength. This shows that it connects to many different topics and appears more frequently across the dataset. Other keywords include "organizational effectiveness" "management science", "personnel management", and "decision making" all indicating strong connections in multiple areas. This suggests that the dataset is focused more on management and organization themes. The top keyword pairings by weight highlight how strong the relationship is between the concepts. E.G- "organizational behaviour" and "organizational effectiveness". Similarily, other high weight pairs showcase that certain topics are studied together. Visually the scatter plot of degree vs strength reveals a clear positive correlation relationship which implies that higher degrees tend to also have higher strengths. 

All in all, the results show that the keyword network is not evenly spread out or distributed. It is dominated by a small number of highly connected keywords that act as central hubs. The hubs represent major research themes in the dataset. Common themes revolve around in the field of organizational and management studies. The keywords that have lower degree and strength appear less frequently as opposed to the highly connected keywords. The strong keywords have a major part in linking different research areas together. 

---

## Conclusion
This project showed how network analysis can be used to reveal patterns in academic keyword data. By creating a weighted co-occurrence network, we were able to identify the most important keywords, strongest relationships, and general structure of the research landscape. The findings reveal that a few central keywords dominate the network connecting to multiple themes across numerous studies. Valuable insights were gained in this project on how things weave and connect together.  
