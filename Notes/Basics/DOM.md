# DOM (Document Object Model)

DOM is a tree-like representation of an HTML document that JavaScript can access and modify.

### Real DOM vs Virtual DOM

**1. Real DOM**

* Represents the actual webpage structure.
* JavaScript can modify DOM elements directly.
* Frequent DOM updates can be costly, depending on the changes.

![DOM Tree](/Images/dom.png)

**2. Virtual DOM**

* React uses an in-memory representation of the UI.
* When state changes, React renders again and compares the new result with the previous one.
* React updates the necessary parts of the actual DOM.

**Remember:** React does not reload the entire DOM for every small change. It updates the DOM where necessary.

![DOM Tree](/Images/Vdom.png)


JSX

# What is JSX?

**JSX (JavaScript XML)** is a syntax extension for JavaScript that allows us to write HTML-like code inside JavaScript.

### Why do we use JSX?

It makes writing and understanding UI code easier in React.

### Example

```jsx
function App() {
  return <h1>Hello World!</h1>;
}
```

Here, JSX allows us to write HTML-like syntax inside a JavaScript function.

### How does JSX work?

1. We write HTML-like code using JSX.
2. A tool like Babel or the build tooling transforms JSX into JavaScript.
3. React uses the resulting JavaScript to create and update the UI.

### Important Rules

* Return a single parent element (or use a Fragment `<>...</>`).
* Use `className` instead of `class`.
* Use `{}` to write JavaScript expressions inside JSX.

**Example:**

```jsx
const name = "Tarun";

function App() {
  return <h1>Hello, {name}!</h1>;
}
```

**Output:** `Hello, Tarun!`
