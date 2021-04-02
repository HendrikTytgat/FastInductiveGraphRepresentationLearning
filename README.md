# FastInductiveGraphRepresentationLearning

This repository contains the implemented Fast Inductive Graph Representation Learning (FIGRL) algorithme described in the [paper of Jiang et al.][paper]

Currently there are three versions implemented in this repository. They all differ in the way the classes deal with the normally distributed random matrix.

The main version in use (implemented as FIGRL), differs from the paper. The algorithm compresses the normally distributed random matrix together with the normalized random walk matrix created in the inductive step. This implementation is the FIGRL class.

## Getting started with this Spectral graph embedding algorithm
(All node IDs for all node types should be transformed to consecutive integer numbers, for instance node type 1 receives the integers from 0 to 1379 and node type 2 from 1380 to 4598)

The requirements for the initialization of this function are the final embedding size and the intermediate dimension used in the compressing stage of the algorithm. The intermediate dimension combined with the final embedding size determine the approximation error for the Fast Inductive Graph Representation Learning algorithm.

Before being able to fit the train data to FIGRL, the data needs to be transformed to a networkX graph. (IMPORTANT NOTE: the order in which the graph is created, is the order that the train embeddings will be generated in)

Perparing for the inductive step or predict function, a networkx graph needs to be created with the training and inductive data (The same important note holds here). The full inductive dataframe for the new incoming nodes for which embeddings are needed. A list of the inductive dataframe columns that are connected node types (ex. [InductiveDataframe.ConnectedNode1,InductiveDataframe.ConnectedNode2,...]). Additionally the maximum id number and the inductive datasets index dataframe should be given.


[paper]: <https://arxiv.org/pdf/1809.08079>
