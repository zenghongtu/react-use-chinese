# `useMap`

React 状态钩子，用于追踪对象型值。


## 用法

```jsx
import {useMap} from 'react-use';

const Demo = () => {
  const [map, {set, reset}] = useMap({
    hello: 'there',
  });

  return (
    <div>
      <pre>{JSON.stringify(map, null, 2)}</pre>
      <button onClick={() => set(String(Date.now()), (new Date()).toJSON())}>Add</button>
      <button onClick={() => reset()}>Reset</button>
    </div>
  );
};
```
