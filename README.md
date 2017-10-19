# CS-101
# Material learned from CS 101 and implementations

#MergeSort:

Divide and conquer method of sorting. First, divide by finding the number q of the position midway between p and r (i.e. add p and r,      divide by 2, and round down), resulting in the subarrays array[p...q] and array[q+1...r]. Next, conquer by recursively (a recursion        algorithm being an algorithm that calls itself with smaller/simpler input values) sort the subarrays. Finally, merge the two sorted     subarrays into a sorted subarray array[p...q]. 
  
#InsertionSort:

A simple algorithm that is less efficient in large lists. Builds the final sorted array one element at a time. 

#SelectionSort:

Also inefficient in large lists. Has O(n^2) time complexity (time complexity quantifying the amount of time taken by an algorithm to run as a function of the length of the string representing the input). Sorts an array by repeatedly finding the minimum element, considering ascending order of elements, from the unsorted part of the array and putting the found element at the beginning. Maintains two subarrays: the sorted array, and the remaining unsorted subarray.


