# WEEK 2 ASSIGNMENT
## PYTHON 101: INTRODUCTION TO PYTHON 

- What is garbage collection iun python and why is it important? How is memory management handled in Python?

Garbage allocation is defined as a memory technique in which a programming language to reclaim memory which is no longer accessible or in use by the application. Garbage allocation is important as it helps allocate memory leaks, allows for optimization of memory use and also ensures that there exists sufficient memory allocation for the program.

Python is an object-oriented programming language which allocates free memory, this is an important aspect as it allows developers not to worry about allocating or deallocating memory in manual format. The best way Python allows for memory management is through use of heap of private spaces. Python manages memory in different ways. Some of these ways include: Memory allocation which automatically allocates memory whenever a new object is allocated. The second way is through Memory Deallocation in which whenever an object is no longer required, Python deallocates the memory allocated to it. The garbage collector frees up memory objects that are no longer in use or referenced by any other program. Garbage collection is another way of automatically freeing up space by objects that no longer use memory.

- What are the key differences between Numpy arrays and python list? List the advantages of using Numpy arrays in numerical computations?
Numpy arrays are defined as powerful python packages useful when working with dimensional data such as one, two or three dimensional data whereas Python Lists is a wide type of data structures that allows programmers to store many different items in a single variable. Code example in action:
  ```
  list_1 = ["London", "Shanghai", "Copenhagen"]
  print(list_1)
   ```
  A line of code for an array would be:
  ```
  array_1d = np.array([1,2,3])
  (array_1d)
    ```

- How does list comprehension work in Python. Provide an example of using it to generate list of squared values or filter based on a condition?
List comprehension is used to create a new list based on the value in an existing iterable objects. List comprehensions usually take the format of:
```
my_list = [expression for element in iterable if condition]
  ```


- Explain the concepts of shallow and  deep copying in Python including when each is approprtiate and how deep copying is implemented?
A shallow copy generates a new object but does not duplicate any objects contained within it. Instead, it copies references to nested objects. If the original object holds references to mutable objects (such as lists or dictionaries), both the original and the shallow copy will point to the same nested objects. Then modifications made to these nested objects in either the original or the shallow copy will affect both, as they share the same references. Deep copying on the other hand involves  creating a full independent duplicate of the original object, also copying all nested objects. As a result, modifications made to the deep copy will not impact the original object, and changes to the original object won't affect the deep copy, since they do not share any object references.

- Explain the differences between Lists and Tuples
List in python is defined as a data structure which helps to store and manipulate an ordered collection of items. Lists more often than not allows for modification of the data structures whereas a Tuple in python is defined as an immutable sequence which can contains elements of any data type. A tuple is notably alike like a List, but the difference remains that they are immutable. I.e cannot be changed.
Example of list in code:
```
x = [0, 1, 2, 3]
x.append(5)
x = [0, 1, 2, 3, 5]
  ```

Example of Tuple in code:
```
my_tuple = (1900, 40.89, 'all', 2006-11-06)
print(my_tuple)
  ```
  
