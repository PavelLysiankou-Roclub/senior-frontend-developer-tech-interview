## Introduction:

The class component defines increment as a regular method.<br>
What issues do you see ?

```ts
class Counter extends React.Component {
    constructor(props) {
        super(props);
        this.state = { count: 0 };
    }

    increment() {
        this.setState({ count: this.state.count + 1 });
    }

    render() {
        return (
            <div>
                <p id="count">Count: {this.state.count}</p>
                <button id="inc" onClick={this.increment}>+</button>
            </div>
        );
    }
}

function App() {
    return <Counter />;
}
```

### Follow-up:

Is this a React issue or a JavaScript issue ? Why ?