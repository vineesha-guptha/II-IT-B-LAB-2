# aim of the experiment
to the find the values in iterative_binary_search
# brief description of binary search
• Sequential search algorithm is very slow if list contains more number of
 elements.
• If the array is not sorted ,linear search is the only solution.
• If the list is sorted , we can use a more efficient algorithm called
 the binary search.
• We should use a binary search whenever the list starts to become large.
• The binary search starts by testing the data in the element at the middle of the list.
• This determines if the target is in first half or second half of the list.
• If it is in first half , we do not need to check the second half.
• If it is in second half , we do not need to check the first half.
• In other words ,either way we eliminate half the list from further
 consideration.
• We repeat this process until we find the target or satisfy ourselves
 that it is not in the list.
• To find the middle of the list we three variables,
one to identify the beginning of the list(first)
one to identify the beginning of the list(mid)
one to identify the beginning of the list(last)
mid=( first + last )/2

# step by step procedure
We basically ignore half of the elements just after one comparison.

Compare x with the middle element.
If x matches with middle element, we return the mid index.
Else If x is greater than the mid element, then x can only lie in right half subarray after the mid element. So we recur for right half.
Else (x is smaller) recur for the left half.

# output obtained


