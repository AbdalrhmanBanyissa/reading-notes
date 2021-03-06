# Functional Programming

## Functional Programming Concepts

> Functional programming is a programming paradigmn -- a style of building the structure and elements of computer programs -- that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data - Wikipedia

Pure functions are the first fundamental concept to learn when we want to understand functional programming. A strict definition of purity:

- It returns the same result if given the same arguments (deterministic)

  - Example: An impure function would receive radius as a parameter and calculate area with PI. If the value of PI were to change, the result of the function changes. A pure function would receive radius and PI as parameters to the function and not have to use an external object to calculate.

  - If the function reads external files, it's not a pure function because the file's contents can change (doesn't return same result)

  - Any function that relies on random number generator can't be pure (doesn't return same result)

* It does not cause observable side effects

  - If the function modifies a global object or parameter passed by reference, the function has observable side effects. Mutability is discouraged in functional programming

    - Example: this function changes the global variable `counter`

      ```javascript
      let counter = 1;

      function increaseCounter(value) {
        counter = value + 1;
      }

      increaseCounter(counter);
      console.log(counter); // 2
      ```

  - To create a pure function that takes in a global object or parameter we reference the value and change it - not the actual object.

    - Example: this function does NOT change the global variable counter

      ```javascript
      let counter = 1;

      function increaseCounter(value) {
        counter = value + 1;
      }

      increaseCounter(counter);
      console.log(counter); // 2
      ```

Pure functions are stable, consistent, and predictable. This makes the code easier to test.

When data is ummutable, its state cannot change after it's created. If you want to change an immutable obejct, you cant. Instead, you create a new object with the new value.

## Refactoring JavaScript for Readability

Good code lives in the middle ground between speed and comprehension.
