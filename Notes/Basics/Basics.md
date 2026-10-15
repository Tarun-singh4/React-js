# What Is React?

React is a **JavaScript library** used to build interactive user interfaces.

### Why do we use React?

* HTML provides structure, CSS provides styling, and JavaScript provides functionality.
* In complex websites, managing UI changes using JavaScript can become difficult.
* React uses reusable components and updates the UI when data changes.
* React can update parts of the UI without reloading the entire webpage.

### What is a Component?

A component is a small, reusable part of a website, such as a Navbar, Footer, or Login Form.

### Library vs Framework

* **Library:** Provides specific functionality that we can use when needed. Example: React.
* **Framework:** Provides a broader structure for building applications. Example: Angular.



<!-- IMPORT AND EXPORT  -->

# JavaScript Modules: Import & Export

### 1. `type="module"`

```html
<script type="module" src="script.js"></script>
```

* Allows us to use `import` and `export` in JavaScript.
* Helps split code into multiple files.
* Modules automatically use strict mode.

### 2. Types of Import/Export

**A. Default Export**

* A file can have only one default export.
* We can give it any name while importing.

`app.js`

```js
export default function greet() {
  console.log("Hello");
}
```

`main.js`

```js
import hello from "./app.js";
hello();
```

**B. Named Export**

* A file can have multiple named exports.
* We normally import using the same exported name.
* Use `{ }` when importing named exports.

`app.js`

```js
export const name = "Tarun";
export const age = 21;
```

`main.js`

```js
import { name, age } from "./app.js";
```

**Remember:**

* Default import → Any name.
* Named import → Same name, using `{ }`.
* You can combine default and named exports in the same file.


ctrl + shift + V