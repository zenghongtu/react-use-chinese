# `useBattery`

React 传感器钩子，用于追踪电池状态。

## 用法

```jsx
import {useBattery} from 'react-use';

const Demo = () => {
  const state = useBattery();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
