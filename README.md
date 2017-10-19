# CS-101
# Material learned from CS 101 and implementations

MergeSort:

Divide and conquer method of sorting. First, divide by finding the number q of the position midway between p and r (i.e. add p and r,      divide by 2, and round down), resulting in the subarrays array[p...q] and array[q+1...r]. Next, conquer by recursively (a recursion        algorithm being an algorithm that calls itself with smaller/simpler input values) sort the subarrays. Finally, merge the two sorted     subarrays into a sorted subarray array[p...q]. 
  
  
InsertionSort:

A simple algorithm that is less efficient in large lists. 
