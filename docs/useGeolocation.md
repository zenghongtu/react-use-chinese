# `useGeolocation`

React 传感器钩子，用于追踪用户地理位置。


## 用法

```jsx
import {useGeolocation} from 'react-use';

const Demo = () => {
  const state = useGeolocation();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
