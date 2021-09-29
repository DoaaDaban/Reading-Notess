# Read: Class 05 Read: 05 - Linked List



If you want to add a node after a given value, follow these steps:

1. add a current node that points at the current node and assign it to the head.

2. create a new node for the value

3. then by using while loop and current.next loop through the linked list

4. create a condition to check if the current node is equal to the value

5. first add a reference for the new node to the current node.next

6. then change the reference for the current node to the new node



A **linked List** is a linear data structure and The elements in a linked are linked using pointers.

![Linked Lists](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200922124319/Singly-Linked-List1.png)

## Types of Linked List:

1. Singly: A node in the singly linked list consist of two parts: data part and link part. Each node contains only next pointer.

2. Doubly: Contains an extra pointer, typically called previous pointer, together with next pointer and data which are there in singly linked list.

## Node 

Nodes are the individual items in linked list and each node contains data and property called `Next` which contains the reference to the next node.

## Head
It is the first node in a linked list.

## Traversal

When traversing a linked list we depend on the next value im each node to guide us where the next reference is pointing. It is important because it leads us to the next node and aloow us to extract the data appropriately.

## Advantages of Linked List

1. Dynamic Data Structure

2. Insertion and Deletion

3. No memory wastage

4. Implementation

## Disadvantages of Linked List

1. Slow Search Time

2. Slow Traversal

3. Use more memory