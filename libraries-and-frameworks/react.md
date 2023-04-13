# React Cheatsheet

## Unique Features

- JavaScript library for building user interfaces
- Component-based architecture
- Virtual DOM
- JSX syntax
- React Router
- Redux

## Components

```javascript
// Define a component
function ComponentName(props) {
    // Component body
    return (
        <div>{props.property}</div>
    );
}

// Render a component
ReactDOM.render(<ComponentName property="value" />, document.getElementById('root'));
```

## State

```javascript
// Define state in a class component
class ComponentName extends React.Component {
    constructor(props) {
        super(props);
        this.state = { property: value };
    }
    render() {
        return (
            <div>{this.state.property}</div>
        );
    }
}

// Update state
this.setState({ property: new_value });
```

## Props

```javascript
// Pass props to a component
<ChildComponent property={value} />

// Access props in a component
function ChildComponent(props) {
    return (
        <div>{props.property}</div>
    );
}
```

## Routing

```javascript
// Define routes
<Router>
    <Switch>
        <Route exact path="/" component={Home} />
        <Route path="/about" component={About} />
    </Switch>
</Router>

// Navigate to a route
<Link to="/about">About</Link>
```

## Redux

```javascript
// Define a store
const store = createStore(reducer);

// Define a reducer
function reducer(state = initialState, action) {
    switch (action.type) {
        case 'ACTION_TYPE':
            return { ...state, property: new_value };
        default:
            return state;
    }
}

// Dispatch an action
store.dispatch({ type: 'ACTION_TYPE', payload: data });

// Connect a component to the store
function mapStateToProps(state) {
    return { property: state.property };
}
export default connect(mapStateToProps)(ComponentName);
```

## Resources

- [React Documentation](https://reactjs.org/docs/getting-started.html)
- [React tutorial](https://reactjs.org/tutorial/tutorial.html)
- [React hooks](https://reactjs.org/docs/hooks-intro.html)
- [React router](https://reactrouter.com/web/guides/quick-start)
- [React Redux](https://redux.js.org/introduction/getting-started)