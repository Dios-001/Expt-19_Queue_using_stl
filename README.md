# EXP 18 - Stack Implementation using Array

This project demonstrates the implementation of a **stack data structure** using arrays. A stack is a **linear data structure** that follows the **Last In First Out (LIFO)** principle, meaning the last element added is the first to be removed.

# Algorithms

## Queue using STL

### Algorithm

1. **Start.**  
2. **Initialize an Empty Queue:**  
   - Create an empty queue `q` of integers.  
3. **Push Elements onto the Queue:**  
   - Push the value `30` onto the queue.  
   - Push the value `20` onto the queue.  
   - Push the value `10` onto the queue.  
4. **Print the Front Element of the Queue Before Pop:**  
   - Output the front element of the queue (Output: `30`).  
5. **Remove the Front Element from the Queue:**  
   - Use `pop()` to remove the front element.  
6. **Print the New Front Element After Pop:**  
   - Output the new front element (Output: `20`).  
7. **End.**

---

## Queue Implementation in Array

### Algorithm

1. **Start.**  
2. **Define the Queue Class:**  
   - Declare attributes:  
     - `capacity` (int)  
     - `front` (int)  
     - `rear` (int)  
     - `arr` (dynamic array)  
3. **Initialize the Queue:**  
   - Create a constructor that sets `front` and `rear` to `-1` and allocates memory based on `capacity`.  
4. **Define Methods:**
   - **push():**  
     - Add an element to the queue if it's not full.  
     - Initialize `front` if the queue was empty.  
   - **pop():**  
     - Remove the front element from the queue if it's not empty.  
     - Reset `front` and `rear` to `-1` if there's only one element left.  
   - **peek():**  
     - Return the front element of the queue if it's not empty.  
     - Otherwise, return `-1`.  
5. **In the Main Function:**  
   - Create a queue `q` with a capacity of `5`.  
   - Push the elements `10`, `20`, and `30` onto the queue.  
   - Print the front element using `peek()` (Output: `10`).  
   - Remove the front element using `pop()`.  
   - Print the new front element after pop (Output: `20`).  
6. **End.**


## Features

- **Push Operation**: Adds an element to the stack.
- **Pop Operation**: Removes the top element from the stack.
- **Peek Operation**: Retrieves the top element without removing it.
- **Overflow & Underflow Handling**: Handles cases when the stack is full or empty.

## Code Overview

This project includes:

- **C++ code using STL (`stack`)** for stack operations.
- Demonstrates basic stack functionalities like pushing, popping, and peeking elements.

### Sample Code

```cpp
#include <iostream>
#include <stack>
using namespace std;

int main() {
    stack<int> st;
    st.push(30);
    st.push(20);
    st.push(10);

    // Print the top element of the stack
    cout << "Top element of the stack: " << st.top() << endl;

    return 0;
}
```
