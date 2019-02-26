# `useMotion`

React 传感器钩子，使用设备的加速度传感器跟踪其运动。


## 用法

```jsx
import {useMotion} from 'react-use';

const Demo = () => {
  const state = useMotion();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
