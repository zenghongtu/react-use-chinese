# `useMediaDevices`

React 传感器钩子，用于跟踪连接的硬件设备。


## 用法

```jsx
import {useMediaDevices} from 'react-use';

const Demo = () => {
  const state = useMediaDevices();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
