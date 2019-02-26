# `useNetwork`

React 传感器钩子，用于跟踪连接的硬件设备。返回：

```json
{
  "online": true,
  "since": "2018-10-27T08:59:05.562Z",
  "downlink": 10,
  "effectiveType": "4g",
  "rtt": 50
}
```

## 用法

```jsx
import {useNetwork} from 'react-use';

const Demo = () => {
  const state = useNetwork();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
