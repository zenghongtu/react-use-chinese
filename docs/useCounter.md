# `useCounter`

React 状态钩子，用于追踪数值型值。

`useNumber` 是 `useCounter` 的别称。

## 用法

```jsx
import {useCounter, useNumber} from 'react-use';

const Demo = () => {
  const [value, {inc, dec, get, set, reset}] = useCounter(5);

  return (
    <div>
      <div>{value} is {get()}</div>
      <button onClick={() => inc()}>Increment</button>
      <button onClick={() => dec()}>Decrement</button>
      <button onClick={() => inc(5)}>Increment (+5)</button>
      <button onClick={() => dec(5)}>Decrement (-5)</button>
      <button onClick={() => set(100)}>Set 100</button>
      <button onClick={() => reset()}>Reset</button>
      <button onClick={() => reset(25)}>Reset (25)</button>
    </div>
  );
};
```
