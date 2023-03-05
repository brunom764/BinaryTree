# BinaryTree
Python implementation of a binary search tree, which puts a searched item at the root of the tree.

## Problem Statement
Modern processors use multiple levels of cache to speed up access to RAM. These caches store the most frequently used information by the processor, 
favoring queries to memory positions that are repeated during the execution of a process. This reduces the average latency between the processor and RAM, 
significantly improving overall system performance.

The CIn Core processor is an example of a processor that has this feature and uses a data structure that is reactive to repetitive queries. 
That is, the more a data is requested, the easier it is to obtain it, as it will be stored in one of the processor's cache levels. 
This further reduces latency and improves processing speed. As an enthusiast of processors, you want to explain this technology to your friends Matheus,
Isabelle, and Arthur, so that they understand how it can improve the performance of their systems.

To be able to explain to your friends, you come to the conclusion that the best thing to do is to use a tree structure,
where with each query to the structure, in addition to delivering the data, the queried data should go to the top. In the excerpt below,
the node with value 5 can be seen rising in the tree.
