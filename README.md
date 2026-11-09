# Exp 9 – React Lab Exercise: React Fragments

## NAME:  AMMINENI MOKSHA SREE  
## REG NO: 2305001001  

## Aim
To understand and implement React Fragments to group multiple JSX elements without creating unnecessary HTML elements in the DOM.

## Objectives
- Understand the concept of React Fragments.
- Use Fragment shorthand syntax.
- Use the explicit Fragment syntax.
- Group multiple JSX elements without an extra DOM node.
- Understand the difference between Fragments and div elements.

## Program

### Step 1: Create a React Project

```bash
npm create vite@latest react-fragments
cd react-fragments
npm install
npm run dev
```

Select React as the framework and JavaScript as the variant.

### Step 2: App.jsx – Using Fragment Shorthand

```
function Student() {
  return (
    <>
      <h2>Student Details</h2>

      <h3>Name: AMMINENI MOKSHA SREE</h3>

      <p>Register Number: 2305001001</p>

      <p>Department: Computer Science and Engineering</p>
    </>
  );
}

function App() {
  return (
    <>
      <h1>College Information System</h1>

      <Student />
    </>
  );
}

export default App;
```

### Step 3: Using Explicit Fragment Syntax

```jsx
import { Fragment } from "react";

function Student() {
  return (
    <Fragment>
      <h2>Student Details</h2>
      <p>Name: AMMINENI MOKSHA SREE</p>
      <p>Department: CSE</p>
    </Fragment>
  );
}

function App() {
  return (
    <Fragment>
      <h1>College Information System</h1>
      <Student />
    </Fragment>
  );
}

export default App;
```

## Output

### Fragment Shorthand Syntax

<img width="1097" height="573" alt="image" src="https://github.com/user-attachments/assets/6b448750-57a8-46cd-8617-a33c5565e9b1" />


### Explicit Fragment Syntax

<img width="1101" height="580" alt="image" src="https://github.com/user-attachments/assets/5e303852-cbd6-4e5c-bca6-01f0ab0b08df" />


## Result

Thus, React Fragments were successfully implemented using shorthand and explicit syntax to group multiple JSX elements without creating unnecessary DOM elements.
