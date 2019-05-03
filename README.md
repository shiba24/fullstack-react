# Fullstack react

Personal note of fullstack react.

# P.1 Your first React Web Application 

## Summary

 1. We think about and organize our React apps as components

 2. UsingJSXinsidetherendermethod

 3. Data flows from parent to children through props

 4. Event flows from children to parent through functions

 5. Utilizing React lifecycle methods

 6. Stateful components and how state is different from props

 7. How to manipulate state while treating it as immutable

## Contents

- `render()` is the only required method for a React component.

```js
class HelloWorld extends React.Component { render() { return        (<p>Hello, world!</p>) }
}
```

- In JSX, you can write values as like in html format, instead of `React.createElement` .

- Developer mode in Chrome: `Command + Option + J`

- Babel turns ES6 code into ES5 code.

- `ReactDOM.render([what], [where])`

- In React, native HTML elements always start with a lowercase letter whereas React component names always start with an uppercase letter.

- `JSX.class` is a reserved word. Therefore, React has us use the attribute name className. Later, when the HTML element reaches the page, this attribute name will be written as class.


- The way data flows from parent to child in React is through **props**. (e.g. `this.props` )

- In JSX, braces are a delimiter, signaling to JSX that what resides in-between the braces is a JavaScript expression. A delimiter for string is '. For number of null types, use braces.

- ES6: Prefer `const` and `let` over `var`.

- `key` property needs to be unique per React component in a list.

- While the child can read its props, it can’t modify them. A child does not own its props.

- Data changes come from the “top” of the app and are propagated “downwards” through its various components.

- We can pass down functions as props too.

- In JavaScript, the special this variable has a different binding depending on the context.

- For the render() function, React binds this to the component for us. Any time we define our own custom component methods, we have to manually bind this to the component ourselves.

- When the state or props of a component update, the component will re-render itself.
Every React component is rendered as a function of its this.props and this.state. 

- state is owned by the component.

- React specifies a set of lifecycle methods.

- The only time we can modify the state in this manner is in constructor(). For all state modifications after the initial state, React provides components the method this.setState().

# P.56 Components

- When you visit a website, assets are the files that your browser downloads and uses to display the page. index.html is delivered to the browser and inside its head tags it specifies which additional files from the server the browser needs to download.

- load in the dependencies within the head tags (the assets).

- Inside of body we have a few elements.

- <div> is where we will ultimately mount our React app.

- <script> tag is where we instruct the browser to load app.js into the page.

- When developing a React app from scratch:

1. Break the app into components

2. Build a static version of the app

3. Determine what should be stateful

4. Determine in which component each piece of state should live 5. Hard-code initial states

6. Add inverse data flow

7. Add server communication



