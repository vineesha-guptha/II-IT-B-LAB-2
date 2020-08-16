# aim of the exeriment
to find the values in recursive_linear_search
# biref description about linear search
• Sequential search is used whenever the list is not ordered.
• Generally we use the technique only for small lists or lists that are
not
 searched often.
• In the sequential search , we start searching for the target from the
 beginning of the list, and we continue until the we find the target or
 until we are sure that it is not in the list.
• This gives us two possibilities:
either we find it or
we reach the end of the list
# step by step procedure
Therefore, the following steps can be followed to compute the answer:

Get the array for which the subsets with the sum equal to K is to be found.
Recursively count the subsets with the sum equal to K in the following way:
# Base Case: 
The base case will be when the end of the array has been reached. If here the sum has been found as X, then increase the count of the subset by 1. Return the count evaluated in the base condition.
# Recursive Call:
If the base case is not satisfied, then call the function twice. Once by including the element at index ‘i’ and once by not including the element. Find the count for both these cases and then return the final count.
count = subsetSum(arr, n, i + 1, sum - arr[i], count);
count = subsetSum(arr, n, i + 1, sum, count);
# Return Statement:
At every step, the count of subsets by either including a particular element or not including a particular element is returned. Finally, when the entire recursion stack is executed, the total count is returned.
From the above approach, it can be clearly analyzed that if there are N elements in the array, then a total of 2N cases arise. Every element is checked for the above cases using recursion.
 # output obtained:
 ![output](out66(2).png) (out0(2).png)
