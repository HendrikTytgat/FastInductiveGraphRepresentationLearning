# FastInductiveGraphRepresentationLearning

This repository contains the implemented Fast Inductive Graph Representation Learning (FIGRL) algorithme described in the [paper of Jiang et al.][paper]

Currently there are three versions implemented in this repository. They all differ in the way the classes deal with the normally distributed random matrix.

The main version in use, compresses this matrix together with the normalized random walk matrix created in the inductive step. This is the FIGRL class.

[paper]: <https://arxiv.org/pdf/1809.08079>