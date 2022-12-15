# Unsupervised Machine Learning on Graphs

Unsupervised machine learning refers to the subset of machine learning algorithms that do not exploit any target information during training. Instead, they work on their own to find clusters, discover patterns, detect anomalies, and solve many other problems for which there is no teacher and no correct answer known a priori.

## Unsupervised graph embedding

Algorithms for graph embedding using unsupervised graph machine learning have been classified as *shallow embedding methods*, *autoencoders*, and *Graph Neural Networks (GNNs)*.

### Shallow embedding methods

Algorithms that are able to learn and return only the embedding values for the learned input data. They all factorize an input graph expressed as a matrix in different components. Examples are:

#### Matriz factorization

The main difference between each method lies in the loss function used during the optimization process.Indeed, different loss functions allow creating an embedding space that emphasizes specific properties of the input graph. Two known algorithms are Graph Factorization (GF) and Higher-Order Proximity Preserved Embedding (HOPE). 

- GF Python example

<ul>

```python
import networkx as nx
from gem.embedding.gf import GraphFactorization
G = nx.barbell_graph(m1=10, m2=4)
gf = GraphFactorization(d=2, data_set=None, max_iter=10000,
eta=1*10**-4, regu=1.0)
gf.learn_embedding(G)
embeddings = gf.get_embedding()
```
</ul>

</ul>