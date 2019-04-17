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


p.15