# A-Network-Analysis-of-Game-of-Thrones

In this notebook, I will look at the character co-occurrence network and its evolution over the five books in R.R. Martin's hugely popular book series A Song of Ice and Fire. The importance of the characters changes over the books using different centrality measures. There are 5 CSV files that covers 5 books of that fiction. Each CSV file has 5 columns: Source, Target, Type, weight, and book#.
![alt text](https://github.com/Alexmxz/A-Network-Analysis-of-Game-of-Thrones/blob/main/GoT.png)   

**Project Tasks**   
**Populate the network with the DataFrame**
1. Use nx.degree_centrality(graph) to calculate the centrality of all nodes
2. Use nx.betweenness_centrality(graph, weight='weight') to calculate the weighted betweenness centrality of all the books.
3. Use nx.pagerank() and create a list of PageRank measures for all the books.
4. Correlation between above 3 method for caluclation importance of characthers in all 5 books.  

![alt text](https://github.com/Alexmxz/A-Network-Analysis-of-Game-of-Thrones/blob/main/Network.png)   


## Code and Resources
**Python Version:** 3.8   
**Packages:** pandas, numpy, matplotlib, seaborn ,networkx




## Networkx Module
networkx provides different kind of graph objects, graph, digraph, multigraph, multidigraph. In this case, you will create a graph because the network is undirected, that is, an edge from character A to character B implies that there exists an edge the other way too, from character B to character A.
![alt text](https://github.com/Alexmxz/A-Network-Analysis-of-Game-of-Thrones/blob/main/graph.png)   

![alt text](https://github.com/Alexmxz/A-Network-Analysis-of-Game-of-Thrones/blob/main/IoC.png) 

## Key takeaways
1.Sorting dic to generate the list of tuples contains [(index,vlaue),...]   
sorted_deg_cen_book1 = sorted(deg_cen_book1.items(), key=lambda x: x[1],reverse=True)[0:10]
2.Iterate through the DataFrame book1 row-wise using iterrows()   

