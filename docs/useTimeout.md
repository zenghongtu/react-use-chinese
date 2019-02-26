# `useTimeout`

在指定的毫秒数后返回 `true`。

## 用法

```jsx
import { useTimeout } from 'react-use';

const Demo = () => {
  const ready = useTimeout(2000);

  return <div>Ready: {ready ? 'Yes' : 'No'}</div>;
};
```
