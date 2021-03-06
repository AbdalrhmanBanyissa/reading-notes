# React and Forms

## React Docs - Forms

* HTML form elements work differently from other DOM elements in React because form elements naturally keep some internal state.

### **Controlled Components**

* In HTML, form elements like `input`, `textarea`, and `select` maintain their own state and update based on user input.

* Make the React state to be the "single source of truth" to have a React component render a from which also controls what happens in that form. This type of form element is called a "controlled component"

* With a controlled component, the input's value is always driven by the React state. You can use this to pass the value of state to other elements too.

### **Controlled Input Null Value**

* Specifying the value prop on a controlled component prevents the user from changing the input unless you want them to be able to.

## React Bootstrap - Forms

The `FormControl` component renders a form control with Bootstrap styling. It wraps a form control with proper spacing, along with support for a label, help text and validation state.
