python program to sort array which consists of 0,1 and 2 without using any sorting algo
Sort the array consisting of 0,1 and 2 Using Python
In this article we will see a Python Program to sort the given array which consist of 0,1,2. User will enter elements of array which is either 0,1 or 2. We have to sort that array consisting o,1 and 2 but without using sorting algorithm. We will use count function to count different elements and then arrange them.

Example:-

Array: 1 2 0 2 1 0 2 1 0 2 0 1
Array after sorting: 0 0 0 0 1 1 1 1 2 2 2 2
Algorithm
Step 1: Declare three variable count_0, count_1 and count_2
Step 2: Using count function, count the number of zero in array and store in count_0
Step 3: Using count function, count the number of one in array and store in count_1
Step 4: Using count function, count the number of two in array and store in count_2
Step 5: Declare an array name new_arr
Step 6: Append all the 0 to new_arr
Step 7: Append all the 1 to new_arr
Step 8: Append all the 2 to new_arr
Step 9: Print new_arr
sort array which consists of 0,1 and 2 without using any sorting algo using python
Python code
Run
def sort(arr):
    # Note: We cannot use sort function
    # we will find the count of 0,1,2 in the given array with help of count function

    count_0 = arr.count(0)
    count_1 = arr.count(1)
    count_2 = arr.count(2)

    # declare new array
    new_arr = []

    # append 0 to new array
    for i in range(count_0):
        new_arr.append(0)

    for i in range(count_1):
        new_arr.append(1)

    for i in range(count_2):
        new_arr.append(2)
    print(" After sorting:", new_arr)


array = [1, 2, 0, 2, 1, 0, 2, 1, 0, 2, 0, 1]
print("Before Sorting:", array)
# call function
sort(array)
Output
Before Sorting: [1, 2, 0, 2, 1, 0, 2, 1, 0, 2, 0, 1]
 After sorting: [0, 0, 0, 0, 1, 1, 1, 1, 2, 2, 2, 2]
