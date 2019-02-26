# `useAsync`

React 钩子，用于解析 `async` 函数或返回 promise 的函数。


## 用法

```jsx
import {useAsync} from 'react-use';

// Returns a Promise that resolves after one second.
const fn = () => new Promise((resolve) => {
  setTimeout(() => {
    resolve('RESOLVED');
  }, 1000);
});

const Demo = () => {
  const state = useAsync(fn);

  return (
    <div>
      {state.loading?
        <div>Loading...</div>
        : state.error?
        <div>Error...</div>
        : <div>Value: {state.value}</div>
      }
    </div>
  );
};
```


## 参考

```ts
useAsync(fn, args?: any[]);
```
