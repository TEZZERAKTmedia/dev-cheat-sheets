# 🟨 TypeScript Cheat Sheet

## 🔤 Basic Types
```ts
let id: number = 5;
let name: string = "Trentyn";
```

## 🔘 Interfaces & Types
```ts
interface User {
  id: number;
  name: string;
}
```

## 🔁 Generics
```ts
function identity<T>(arg: T): T {
  return arg;
}
```

## ✅ React Props
```ts
type Props = { title: string };
const Header: React.FC<Props> = ({ title }) => <h1>{title}</h1>;
```