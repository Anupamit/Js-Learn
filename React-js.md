# Table of Contents

- [React](#What-is-React?)

# What is React?
- React is refer as js framework.
- Created by Facebook.
- It's a tool of building UI components.
- It's work as Virtual Dom in memory.
- It's use as unidirectional one way data binding.

# what is Dom?
- Dom is stand for Document Object model.
- The representation of entire user interface of a web application as a tree data structure.
- It's classify as two parts (a)Virtual Dom  (b)Real Dom

# What is JSX?
- JSX enables and simplifies the creation of HTML in React.
- JSX stands for JavaScript XML.
- JSX converts HTML tags into react elements.
- JSX you can write expressions inside curly braces { }.
- JSX is a JavaScript Extension Syntax used in React to easily write HTML and JavaScript together.

            const jsx = <h1>This is JSX</h1>

# What are Components?
- Components are like functions that return HTML elements.
- Components are independent and reusable bits of code. 
  They serve the same purpose as JavaScript functions, but work in isolation and return HTML.
- There are two kinds of components in React: functional and class components.

# What is a Class Component?
- Class components are ES6 classes that return JSX and necessitate the use of React extensions.

            import React, { Component } from 'react'
            export default class App extends Component {
            render() {
            return (
                  <div>
                  <h1>Hello World</h1>
                  </div>
            )
            }
            }

# What is a Functional Component?
- A Function component also returns HTML, and behaves much the same way as a Class component,
  but Function components can be written using much less code, are easier to understand.
- A JavaScript/ES6 function that returns a React element is referred to as a functional component (JSX).
- Since the introduction of React Hooks, we have been able to use states in functional components.

            function Car() {
            return <h2>Hi, I am a Car!</h2>;
            }

# What is rendering a component?
- Back Example of React application has a component called Car, which returns an `<h2>` element.
- To use of this component in your application, use similar syntax as normal HTML: `<Car />`

            const root = ReactDOM.createRoot(document.getElementById('root'));
            root.render(<Car />);

# What is Props?
- Props are like function arguments, and you send them into the component as attributes in html.
- Components can be passed as props, which stands for properties.
- They are used to transfer data from one component to the next (parent component to child component).
- They are typically used to render dynamically generated data.

            function Car(props) {
            return <h2>I am a {props.color} Car!</h2>;
            }
            const root = ReactDOM.createRoot(document.getElementById('root'));
            root.render(<Car color="red"/>);

# How to Use CSS in React?
- There are 3 ways to style a react application with CSS:
   - Inline Styles
   - External Styling
   - CSS in JS

# What is react event?
- React has the same events as HTML: click, change, mouseover etc.
- React events are written in camelCase syntax: `onClick` instead of `onclick`.
- React event handlers are written inside curly braces: `onClick={damm}`  instead of `onClick="damm()"`.
- To pass an argument to an event handler, use an arrow function.

# what is react list?
- In React, you will render lists with some type of loop. The JS map() array method is generally the preferred method.