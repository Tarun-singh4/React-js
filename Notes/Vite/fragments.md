What Are Fragments in JSX?

A component must return a single enclosing element. Fragments let us group multiple elements without adding an extra DOM element.

Without Fragment ❌
function App() {
  return (
    <div>
      <h1>Hello</h1>
      <p>Welcome to React!</p>
    </div>
  );
}
With Fragment ✅
function App() {
  return (
    <>
      <h1>Hello</h1>
      <p>Welcome to React!</p>
    </>
  );
}
Remember
<>...</> is shorthand for a React Fragment.
Fragments group multiple elements without adding an extra DOM node.



writting an function in react

we can call functions like 
hello()
<hello />



rafce

import React from 'react'

const App = () => {
  return (
    <div>App</div>
  )
}

export default App