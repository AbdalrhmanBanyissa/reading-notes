# In Memory Storage

## Understanding the JavaScript Call Stack

## CALL STACK

- The JavaScript engine is a single-threaded interpreter comprising of a heap and a single call stack. (It can only do one thing at a time)

- The call stack is primarily used for invoking functions. The call stack is synchronous, so the function execution is done one-at-a-time from top to bottom.

- A call stack is a data structure that uses the LIFO principle (last in, first out) to temporarily store and manage function invocation (calling the function). The last function that gets pushed into the stack is the first to be popped out when the function returns.

- When a function is invoked, the function + its parameters & variables are pushed into the call stack - to form a stack frame.

  - This stack frame is a memory location in the stack.
    - The memory is cleared when the function returns as it is popped out of the stack.

- The call stack maintains a record of the position of each stack frame, and when one function is executed it is removed and moves on to the next one.

### Stack Overflow

- A stack overflow happens when there is a function that calls itself (recursive function) with no exit point. The browser will run it until it exceeds the maximum call stack size.

## JavaScript Error Messages

### Reference Errors

- When you try to use a variable that isn't declared

- Common thing when using const and let - there is a time between the hoisting and being declared

  - A fix for these is to declare the variable before a declaration is made:

        ```javascript
        let foo;
        foo = "Hello";
        ```

### Syntax Errors

- When you have something that can't be parsed in terms of syntax
  - Can be solved by fixing the syntax

### Range Errors

- Manipulating with an invalid length
  - An array cannot have a negative length

### Type Errors

- When the data types you're trying to use or access are incompatible

  - Like accessing a property in an undefined type of variable

- Probably the most frequent error in JavaScript.

  - To fix, make sure the property exists before trying to access it.
