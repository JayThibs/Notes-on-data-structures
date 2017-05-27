This will be a collection of notes on data structures. I'm taking these notes to review different data structures and cement my knowledge. If anyone wants to use this as a guide, that's even better.

A big portion of the notes will come from the data structures course by mycodingschool: https://www.youtube.com/playlist?list=PL2_aWCzGMAwI3W_JlcBbtYTwiQSsOTa6P

# Introduction to Data Structures

* A dictionary needs to be in a certain order for it to be practical to use.
* A city map needs to be visual with landmarks in order to understand what we’re looking at.
* A cashbook in accounts needs to be organized in columns and rows that have values assigned to them. It is easier to manipulate and understand the data in this way.

<b>A data structure is a way to store and organize data in a computer so that it can be used efficiently.</b>

We'll talk about data structures as:

1. Mathematical and logical model -> or abstract data types. For example, a television can be turned on and off, receive signals, has audio and video -> this is an abstract view.

An abstract data type for example would be a list that can:
- Store a given number of elements of any type
- Read elements by position
- Modify element at a position
2. Implementation: Implementation is a term used across computer science. When someone talks about implementation, they are talking about how a specific idea or concept is actually written in code.

<b>Abstract data types (ADTs) define data and operations</b>, but <i>no implementation</i>.

Some of the data structures that exist are:

* Arrays
* Linked list
* Stack
* Queue
* Tree
* Graph
* and more…

When we study these data structures, we will study the:

1. Logical view
2. Operations (what operations are available to us using these data structure)
3. Cost of operations (how much time does it take to do a specific operation on a data structure)
4. Implementation

<b>Data Structures: List as abstract data types</b>

A basic list would be an array. We can use arrays when we want to have:

1. a list with a specific number of elements of a given data types. This is a static list and we will know the number of elements before creating the list. Be able to write/modify elements at a position. Read element at a position.

2. a dynamic list that can grow as need be. You make a empty list of size 0 and then insert / remove / count / read / modify / specify the data type of the list. We need to write more operations on top of arrays to provide this functionality. We need to create a max size empty array that will contain all the values, but still have room for more elements. If we have reached the max size, we need to make this array equal to a new array of bigger size. You should create an array of 2 times bigger (there is a theoretical reason for this exact size). Then we free the memory of the previous array.

#1 is the best use case for arrays. However, #2 will be costly especially if we are dealing with larger arrays. There will either be unused memory (empty cells) or when you apply operations, it will be very inefficient. It is better to use linked lists in the case of #2.

When we apply a certain operations, the cost of the operations on the array are important in deciding on which lists to use. If we use:

* Access - Read/write element at an index which takes constant time: O(1)
* Insert - At the end of the list, it will be constant time, but if we want to insert at a particular point in the list, we will need to shift all of the numbers and so the time is proportional to the size of the list n: O(n)
* Remove - Same as inserting: O(n)
* Adding element - similar to insert, but the array is full and you want to add an element: O(n)

Note:
O(1) = constant time
O(n) = time proportional to the size of the array

# Introduction to linked lists

