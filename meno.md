# React TODO App
 
環境を構築する
今回はViteを使用してReactの環境を構築する

```
npm create vite@latest
``` 

ネームドエクスポートを使用

```
export const Todo = () => {
  return <div>Todo</div>
};
```     
合わせて、src/main.tsxを作成する

```
import React from "react";
import ReactDOM from "react-dom/client";
import { Todo } from "./Todo";

const rootElement = document.getElementById("root")!;
const root = ReactDOM.createRoot(rootElement);

root.render(
  <React.StrictMode>
    <Todo />
  </React.StrictMode>
);
``` 
useEffectを使用して、Todoを表示する

```
useEffect(() => {
  console.log("Todo");
}, []);
```
