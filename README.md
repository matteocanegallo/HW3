# HW3
In this file I implemented 4 different classes that keeps track of the minimum and maximum number of a list where random numbers are added. Each class use a different function to sort the list.
Our goal is to measure the average time of execution that each class takes to:1)Add a number 2)Get the minimum 3)Get the maximum. Once obtained these results we want to produce plots which show the performances of the different algorithms.

The first class, 'MinMaxQuick', use the function quicksort to sort the list. It is a recursive algorithm that use the 'divide and conquer' method: in the 'divide step' a pivot is choosen, the list is divided into subarrays with elements smaller than the pivot and elements greater than the pivot. This procedure, called partitioning is made recursively selecting every time a new pivot for the subarrays. In the second step , 'conquer', the subarray are recursively sorted and then all the subarray are rejoined and the list sorted is obtained.

The second class, 'MinMaxTree', use the data structure Binary Tree to sort the list.Binary trees organize data depending on the values of the elements:
-elements that are less than the parent are found in the left subtree
-elements that are greater than the parent are found in the right subtree
It is composed of nodes connected by edges. The first node is called 'root node',each node is associated with at most 2 children and every node other than the root is associated with one parent node. Every time we add a node to the Tree, the function compares the value of the node to the parent node and decides to add it as a left node or a right node.

The third class, 'MinMaxHeap', use the heap data structure. The property of this data structure is that each time a number is added through the function heappush, the order is adjusted, so that heap structure is maintained.

The fourth class, 'MinMaxBubble', use the function BubbleSort. It compares adjacent items and exchanges those that are out of order. Each pass through the list places the next largest value in its proper place. In essence, each item “bubbles” up to the location where it belongs.

Then the function 'measure time' is defined to time the time required to add a number, get the minimum and the maximum.

