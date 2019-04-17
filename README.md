# Fullstack react

Personal note of fullstack react.

# 1. First react application

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

-
