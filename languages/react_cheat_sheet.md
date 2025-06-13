# ⚛️ React Cheat Sheet

## 📦 State and Props
```js
const [count, setCount] = useState(0);
```

## 🔁 useEffect
```js
useEffect(() => {
  fetchData();
}, []);
```

## 🧩 useContext
```js
const value = useContext(MyContext);
```

## 🔁 Routing
```jsx
<BrowserRouter>
  <Route path="/about" component={About} />
</BrowserRouter>
```

## 🛠 Component Structure
```jsx
function MyComponent({ title }) {
  return <h1>{title}</h1>;
}
```