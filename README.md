# EXP 18 - Stack Implementation using Array

This project demonstrates the implementation of a **stack data structure** using arrays. A stack is a **linear data structure** that follows the **Last In First Out (LIFO)** principle, meaning the last element added is the first to be removed.

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
