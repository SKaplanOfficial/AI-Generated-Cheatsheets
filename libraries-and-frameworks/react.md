# React Cheatsheet

## Unique features
- Declarative programming
- Virtual DOM
- Component-based architecture
- One-way data flow
- JSX syntax

## Variables
```jsx
const myVariable = 'Hello, World!';
```

## Functions
```jsx
function myFunction() {
  // function body
}

const myArrowFunction = () => {
  // function body
};
```

## Loops
```jsx
{myArray.map((item) => (
  <MyComponent key={item.id} prop={item.prop} />
))}
```

## Conditionals
```jsx
{isTrue ? <TrueComponent /> : <FalseComponent />}
```

## File manipulation
```jsx
import MyComponent from './MyComponent';

export default function App() {
  return <MyComponent />;
}
```

## Resources
- [React documentation](https://reactjs.org/docs/getting-started.html)
- [React tutorial](https://reactjs.org/tutorial/tutorial.html)
- [React hooks](https://reactjs.org/docs/hooks-intro.html)
- [React router](https://reactrouter.com/web/guides/quick-start)
- [React Redux](https://redux.js.org/introduction/getting-started)