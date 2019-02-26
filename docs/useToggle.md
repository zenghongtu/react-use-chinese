# `useToggle`

React 状态钩子，用于追踪布尔型值。

 `useBoolean` 是 `useToggle` 的别称。


## 用法

```jsx
import {useToggle, useBoolean} from 'react-use';

const Demo = () => {
  const [on, toggle] = useToggle(true);

  return (
    <div>
      <div>{on ? 'ON' : 'OFF'}</div>
      <button onClick={() => toggle()}>Toggle</button>
      <button onClick={() => toggle(true)}>set ON</button>
      <button onClick={() => toggle(false)}>set OFF</button>
    </div>
  );
};
```
