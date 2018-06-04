# Minions: Fast GPU-based Computation Engine for Small Graphs

## Motivation
Small graphs are prevalent in many real world applications, such as biological analysis, software management, and signal processing. Unfortunately, conventional graph platforms, are designed to accommodate big graphs. If these systems are applied to small graphs, not only the resources and power are wasted but also unnecessarily long processing time is suffered. 

## What is Minions?
Minions is the first Graphics Processing Unit (GPU)-based small graph engine that specially optimized for small graph analytics. 

<img src="picture/minions_work_together.png" class="img-thumbnail" width="300px" style="float:right; margin-left:30px; margin-top:50px; margin-bottom:10px;">

## How Minions Work
Firstly, Minions carefully schedules each GPU thread block to work on one independent task, which yields a twin benefit: caching the most randomly accessed algorithmic metadata in fast GPU shared memory in order to minimize random global memory access and eliminating the expensive inter-block thread synchronization. Second, we construct a runtime arbiter that unveils the size limit of the graph that can be handled by Minions. 


## Evaluation Results
We evaluate Minions with as many as 1, 048 graph datasets and demonstrate that Minions can outperform both CPU- and GPU- based graph frameworks by orders of magnitude. Most notably, Minions is 239× faster than Gunrock, the state-of-the-art GPU-based graph computing framework.


## Source Code
Minions is implemented with CUDA and C++. The source code will be released soon.

## Dataset
[1] [PGR - Protein Graph Repository](http://wjdi.bioinfo.uqam.ca/)

[2] [KONECT - The Koblenz Network Collection](http://konect.uni-koblenz.de/networks/)

[3] [SNAP - Stanford Large Network Dataset Collection](http://snap.stanford.edu/data/index.html)

