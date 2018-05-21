# Minions: Fast Small Graph Engine on GPU

Minions is a small graph engine that runs on GPUs. Minions is built on the key insight that the majority of the graphs in the real world are either very small or can be decomposed into several small subgraphs for computation. Unfortunately, conventional graph platforms, are designed for big graphs, and if applied to these small graphs, not only waste resources and power but also introduce unnecessarily long processing time. Minions identifies this mismatch and proposes to carefully schedule each GPU thread block to work on each independent task and further caches the computation metadata in fast GPU component to remove both global thread synchronization and random global memory access.


The source code will be released soon.


