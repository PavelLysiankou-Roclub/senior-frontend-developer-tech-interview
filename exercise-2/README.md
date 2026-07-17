## Introduction:

Imagine this code was submitted in a pull request.<br>
What issues do you see ?

```ts
function App() {
    const [count, setCount] = useState(0);

    const increment = () => {
        setCount(count + 1);
    };

    const addThree = () => {
        increment();
        increment();
        increment();
    };

    return (
        <div>
            <h2 id="count">Count: {count}</h2>
            <button id="increment" onClick={increment}>Increment</button>
            <button id="add-three" onClick={addThree}>Add 3</button>
        </div>
    );
}
```

### Follow-up:

How many times do you expect this component to re-render after clicking `Add 3`, and why?