## Introduction: 

Imagine this code was submitted in a pull request.<br> 
What issues do you see ?

```ts
function App() {
  const [name, setName] = useState('');

  return (
    <div>
      <input id="name" value={name} placeholder="Type your name" />
      <p id="display">Hello, {name || '...'}!</p>
    </div>
  );
}
```

### Follow-up:

If typing causes expensive re-renders, what optimizations would you apply ?
