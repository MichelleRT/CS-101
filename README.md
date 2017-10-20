# CS-101
# Basic Algorithms, Common Abstract Data Types, Complexity Analysis, etc.

#MergeSort

Divide and conquer method of sorting. First, divide by finding the number q of the position midway between p and r (i.e. add p and r,    divide by 2, and round down), resulting in the subarrays array[p..q] and array[q+1..r]. Next, conquer by recursively (a recursion      algorithm being an algorithm that calls itself with smaller/simpler input values) sort the subarrays. Finally, merge the two sorted     subarrays into a sorted subarray array[p..q]. 
  
#InsertionSort

A simple algorithm that is less efficient in large lists. Builds the final sorted array one element at a time. Similar to SelectionSort, except sorts one element at a time, then places smaller element in the correct place; whereas SelectionSort finds the minimum element, then places the found element in the correct place. 

#SelectionSort

Also inefficient in large lists. Has O(n^2) time complexity (time complexity quantifying the amount of time taken by an algorithm to run as a function of the length of the string representing the input). Sorts an array by repeatedly finding the minimum element, considering ascending order of elements, from the unsorted part of the array and putting the found element at the beginning. Maintains two subarrays: the sorted array, and the remaining unsorted subarray.

#Dijkstra's (Shortest Path) Algorithm

Finds the shortest path tree from the starting vertex (the source), to another point or all other points in the graph by building a set of nodes that have minimum distance from the source. This algorithm avoids edges with a large weight. One stipulation to using the algorithm is that the graph needs to have a nonnegative weight on every edge, but the weighted graph can be either directed or undirected. 

Example: 

#note that Q is the queue of all nodes in the graph,  
#while S is an empty set, to indicate which nodes the algorithm has visited, 
#and nodes/vertices are denoted by u or v 
#so (u, v) is an edge and w(u, v) is the weight of the edge

     function Dijkstra(Graph, source){
         dist[source] = 0                     // Distance from source to source is set to 0
         for each vertex v in Graph:            // Initializations
             if v != source
                 dist[v] = infinity           // Unknown distance function from source to each node set to infinity
             add v to Q                         // All nodes initially in Q
             
       while Q is not empty:                  // The main loop
            v = vertex in Q with min dist[v]  // In the first run-through, this vertex is the source node
            remove v from Q 

            for each neighbor u of v:           // where neighbor u has not yet been removed from Q.
                a = dist[v] + length(v, u)
                if a < dist[u]               // A shorter path to u has been found
                    dist[u] = a            // Update distance of u 

       return dist[]
     end function
     }




