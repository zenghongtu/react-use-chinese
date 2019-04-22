# `useAsyncFn`

React hook that returns state and a callback for an `async` function or a
function that returns a promise. The state is of the same shape as `useAsync`.

 React钩子返回状态和`async`函数或返回promise的函数的回调。 状态与`useAsync`的形状相同。

## Usage

```jsx
import {useAsyncFn} from 'react-use';

const Demo = (url) => {
  const [state, fetch] = useAsyncFn(async () => {
    const response = await fetch(url);
    const result = await response.text();
    return result
  }, [url]);

  return (
    <div>
      {state.loading
        ? <div>Loading...</div>
        : state.error
          ? <div>Error: {state.error.message}</div>
          : state.value && <div>Value: {state.value}</div>
      }
      <button onClick={() => fetch()}>Start loading</button>
    </div>
  );
};
```

## Reference

```ts
useAsyncFn(fn, deps?: any[]);
```
