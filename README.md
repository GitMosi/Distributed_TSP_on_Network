# Distributed_TSP_on_Network

This repository contains a Python implementation of the Distributed Traveling Salesman Problem (TSP) using heuristics and parallel processing concepts. The code utilizes the [python-tsp](https://python-tsp.readthedocs.io/) library for simulated annealing to solve TSP problems.

## Description

The Traveling Salesman Problem (TSP) is a classic optimization problem where the goal is to find the shortest possible route that visits a set of nodes exactly once and returns to the origin node. In this project, we distribute the workload among multiple 'computers' (simulated by splitting the nodes into clusters) and apply a heuristic approach to optimize the routes.

### Key Features

- **Random Node Generation:** Nodes representing cities are generated randomly within a specified coordinate limit.
- **Distance Calculation:** Computes the Euclidean distance matrix using pairwise distance calculations.
- **Local Optimization:** Each computer/cluster uses simulated annealing to optimize its route.
- **Cluster Sorting and Connection:** Clusters are sorted and connected, combining local optimizations into a general TSP solution.
- **Visualization:** Generates a plot to visualize the sorted paths and connections between clusters.

## Requirements

To run this project, ensure you have the following packages installed:

- `numpy`
- `matplotlib`
- `scipy`
- `python-tsp`
