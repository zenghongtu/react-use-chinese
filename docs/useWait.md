# `useWait`

`useWait` 是一个 React 钩子，可以帮助管理页面上的多个加载状态而不会产生任何冲突。它基于一个通过管理多个加载状态 `Array` 的简单想法。内置的 Wait 组件监听其注册的加载器并立即进入加载状态。

## 用法

```jsx
import { useWait } from 'react-use'

function UserCreateButton() {
  const { startWaiting, endWaiting, isWaiting, Wait } = useWait();

  return (
    <button
      onClick={() => startWaiting("creating user")}
      disabled={isWaiting("creating user")}
    >
      <Wait on="creating user" fallback={<div>Creating user!</div>}>
        Create User
      </Wait>
    </button>
  );
}
```

你应该用 `Waiter` 组件包装你的 `App`。它其实是一个 `Context.Provider`，提供一个加载上下文给组件树。

```jsx
const rootElement = document.getElementById("root");
ReactDOM.render(
  <useWait.Waiter>
    <App />
  </useWait.Waiter>,
  rootElement
);
```
