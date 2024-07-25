pair with given sum in python
Pairs with given sum in Python
We will get an array as input from user. We need to find all possible pairs from the given array whose sum is same as given sum. 

Example:

Array :   [5, 2, 3, 4, 1, 6, 7]
Sum= 7
Possible pairs:  [5, 2], [3, 4], [1, 6]


Algorithm
Step 1: Initialize array and its values
Step 2: Initialize value of sum
Step 3: Call the function find
Algorithm for function find
Step 1: Iterate on the elements of array with variable i, from 0 to length of array.
                 1. For each value of i iterate on array from index i till length of array using variable j.

                 2. Check if array[i]+array[j] ==given sum.

                  3. If the above(2) condition is true then print the pairs

python program to find pairs with given sum
Python Code
Run
def find(array, len, summ):
    print("Pairs whose sum is : ", summ)
    for i in range(len):
        for j in range(i, len):
            if (array[i] + array[j]) == summ:
                print(array[i], array[j])


array = [5, 2, 3, 4, 1, 6, 7]

# Take sum as input from user
summ = 7

# print array
print("Array= ", array)

# call function find
find(array, len(array), summ)
Output
Array= [5, 2, 3, 4, 1, 6, 7]
Pairs whose sum is : 7
5 2
3 4
1 6
