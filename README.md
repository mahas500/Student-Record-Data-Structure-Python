**Problem**

A student record consists of:
Student Number (8 digits)
Name
Course code (7 characters)

Administrators would like to register students for courses in any order.
They would like to process students in student number order.
You must create an appropriate data structure for use in an application, which accepts student records as inputs i.e. add(self,student), and stores them so that retrieve() will give the student record with the lowest student number, removing it from the collection. 

Please consider execution (retrieval) time, i.e. keep the records sorted.


**Choice of sorting algorithms**

**Quicksort** is a good choice for large data sets hence I selected it. As I am generating random data set hence the probability is
very less that I will be getting a sorted list as Quicksort is having Worst time complexity of O(n^2) for sorted list. In this case
time complexity will be nlogn.

**Insertion sort** is a good choice now as we have a sorted list now as it will (nlogn) time complexity. Using Quicksort is not a good option here as we will get max depth reached exception if data sets is having 1000 elements because recursion function of quicksort will be called 1000 times as a result we will get a stack overflow condition.
