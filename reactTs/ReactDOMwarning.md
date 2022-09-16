
> if ReactDOM warning with React

```tsx
// 1) Import ReactDOM library
import ReactDOM from 'react-dom/client';

// 2) Get a reference to the div with ID root
const el = document.getElementById('root');

// 3) Tell React to take control of that element
const root = ReactDOM.createRoot(el!);

// 4) Create a component
const App = () => {
  return (
    <div>
      <h1>Hi there!</h1>
    </div>
  );
};

// 5) Show the component on the screen
root.render(<App />);
```

> Important - Due to a bug in the DefinitelyTyped ReactDOM definitions, you need to add the ! operator here:

```tsx
const root = ReactDOM.createRoot(el!);
```
