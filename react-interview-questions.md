Core React

1. What is React?

React is an open-source frontend JavaScript library which is used for building user interfaces especially for single page applications. It is used for handling view layer for web and mobile apps.

2. What are the major features of React?

The major features of React are:
It uses VirtualDOM instead of RealDOM considering that RealDOM manipulations are expensive.
Supports server-side rendering.
Follows Unidirectional data flow or data binding.
Uses reusable/composable UI components to develop the view.

3. What is the difference between Element and Component?

An Element is a plain object describing what you want to appear on the screen in terms of the DOM nodes or other components. Elements can contain other Elements in their props. Creating a React element is cheap. Once an element is created, it is never mutated.

Whereas a component can be declared in several different ways. It can be a class with a render() method. Alternatively, in simple cases, it can be defined as a function. In either case, it takes props as an input, and returns a JSX tree.

4. How to create components in React?
There are two possible ways to create a component.

Function Components: This is the simplest way to create a component. Those are pure JavaScript functions that accept props object as first parameter and return React elements:

function Greeting({ message }) {
  return <h1>{`Hello, ${message}`}</h1>

}
Class Components: You can also use ES6 class to define a component. The above function component can be written as:

class Greeting extends React.Component {
  render() {
    return <h1>{`Hello, ${this.props.message}`}</h1>
  }
}


