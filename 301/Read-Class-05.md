# Putting it all together

## React Docs - thinking in React

* React is the premier way to build big, fast web apps with JavaScript. It makes you think about apps as you build them.

## Process for building a searchable product data table using React

1. Break the UI into a component hierarchy

    Draw boxes around every component - and subcomponent - in the mock and give them all names. How do you know what should be its own component? SINGLE RESPONSIBILITY PRINCIPLE. Ideally, components should only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

2. Build a static version in React

    The easiest way is to build a version that takes your data model and renders the UI but has no interactivity.

    It's best to decouple these processes because building a static version requires a lot of typing and no thinking, and adding interactivity requires a lot of thinking and not a lot of typing.

    Don't use state to build the static version State is reserved only for interactivity and a static version of an app doesn't need a state.

3. Identify the minimal (but complete) Representation of the UI state

    To make your UI interactive, you need to be able to trigger changes to your underlying data model. React does this with state.

    Ask three questions about each piece of data to find state:

    Is it passed in from a parent via props? (If so, it probably isn't state.)
    Does it remain unchanged over time? (If so, it probably isn't state.)
    Can you compute it based on any other state or props in your component? (If so, it isn't state).

4. Identify where your state should live

    After identifying the minimal set of the app state, figure out which component mutates it (owns it). This can often be the most challenging part for new React users to understand.

    For each piece of state in your application:

    * Identify every component that renders something based on its state

    * Find a common owner component (a single component ABOVE all the components that need the state)

    * Either the common owner, or another componenet higher up in the hierarchy should own the state.

    * If you can't find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

5. Add inverse data flow
