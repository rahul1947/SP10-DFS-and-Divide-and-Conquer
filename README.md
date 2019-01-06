## Short Project SP10: DFS and Divide and Conquer
1. Implementation of DFS - strongly connected components on a Directed Graph, 
   using same Object Oriented approach from SP08. 
2. Implementation of two versions of partition algorithms of Quick Sort and 
   their comparison. 
3. Implementation of Dual-Pivot Quick Sort Algorithm.
4. Problem: void rearrageMinusPlus(int[] A)
5. Problem: int[] findKMissing(int[] A)

#### Author
* [Rahul Nalawade](https://github.com/rahul1947)

#### Date
* Nov 11, 2018

_______________________________________________________________________________
### Problems:

#### A. Team Task - Depth First Search: 

**Problem 1.** 
   Implement the algorithm to find strongly connected components of a directed graph.
   Add the method to your DFS class from SP8.  Make changes so that all methods share
   as much of the code as possible.
```
   public static DFS stronglyConnectedComponents(Graph g) { ... }
```

**Solution:** [DFS.java](https://github.com/rahul1947/SP10-DFS-and-Divide-and-Conquer/blob/master/DFS.java)
```
# SP10 - STRONGLY CONNECTED COMPONENTS: 
____________________________________________________________
Graph: n: 11, m: 17, directed: true, Edge weights: false
1 :  (1,11)
2 :  (2,3) (2,7)
3 :  (3,10)
4 :  (4,1) (4,9)
5 :  (5,4) (5,7) (5,8)
6 :  (6,3)
7 :  (7,8)
8 :  (8,2)
9 :  (9,11)
10 :  (10,6)
11 :  (11,3) (11,4) (11,6)
____________________________________________________________
Number of strongly connected components: 4
u	cno
1	3
2	2
3	4
4	3
5	1
6	4
7	2
8	2
9	3
10	4
11	3

# SP08 - CONNECTED COMPONENTS AND TOPOLOGICAL ORDERINGS: 
____________________________________________________________
Graph: n: 10, m: 12, directed: true, Edge weights: false
1 :  (1,3) (1,8)
2 :  (2,4)
3 :  (3,2)
4 :  (4,7)
5 :  (5,10) (5,4)
6 :  (6,8) (6,10)
7 : 
8 :  (8,2) (8,5)
9 : 
10 :  (10,9)
____________________________________________________________
Number of connected components: 2
u	cno
1	1
2	1
3	1
4	1
5	1
6	2
7	1
8	1
9	1
10	1

Topological Ordering 1: 
6 1 8 5 10 9 3 2 4 7 

Topological Ordering 2: 
1 6 3 8 2 5 10 4 9 7 
```

#### B. Optional Task (individual) - Divide and Conquer: 

**Problem 2.**
   Compare the performance of the two versions of partition discussed in class
   on the running time of Quick sort, on arrays with distinct elements.
   Try arrays that are randomly ordered (by shuffle) and arrays in
   descending order.

**Solution:** -


**Problem 3.**
   Implement dual-pivot quick sort.  Like in merge sort, use a threshold 
   (17, say) and stop the recursion when the array size goes below that 
   threshold. Call insertion sort, just once, at the end of the algorithm:
```
   void quickSort(A):
        quickSort(A, 0, A.length-1)
        insertionSort(A, 0, A.length-1)
```
   Compare its performance with merge sort (take 3).  Use arrays with distinct 
   values and arrays with duplicates.

**Solution:** -


**Problem 4.**
   Reorder an int array A[] by moving negative elements to the front, followed 
   by its positive elements.  The relative order of positive numbers must be 
   the same as in the given array.  Similarly, the relative order of its 
   negative numbers should also be retained.  Write an algorithm that runs in 
   O(nlogn), and uses only O(1) extra space (for variables), but can use 
   O(log n) space for recursion.
```
   void rearrangeMinusPlus(int[] arr) { ... }
```

**Solution:** -


**Problem 5.**
   Given an array of n distinct integers, in sorted order, starting
   at 1 and ending with n+k, find the k missing numbers in the sequence. 
   Your algorithm should run in O(k log(n)) time.  Note that a simple
   linear scan of the array can find the answer, but it will not meet
   the requirement on the running time.
```
   // Value of k can be deduced from the last element of the array and arr.length
   int[] missing(int[] arr) { ... }
``` 

**Solution:** -
