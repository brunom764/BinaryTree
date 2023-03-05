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


## Input
Multiple lines with the following operations:

ADD V - Adds a value V to the structure.

SCH V - Searches for the value V in the structure.

## Output
For the ADD operation:

CL(current level) - Where CL represents the level at which the data V was inserted.

For the SCH operation:

PL(previous level) - Where PL represents the level at which the data V was before it went to the top or -1 if the value does not exist in the structure.


## Examples
### Case: 1
#### Input
ADD 165544
ADD 11623
SCH 165544
SCH 165544
SCH 11623

#### Output
0
1
0
0
1

### Case: 2
#### Input
ADD 100
ADD 50
ADD 25
ADD 10
SCH 10
SCH 55
SCH 50
SCH 50

#### Output
0
1
2
3
3
-1
2
0
