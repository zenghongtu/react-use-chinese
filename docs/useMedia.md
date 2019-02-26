# `useMedia`

React 传感器钩子，用于跟踪CSS媒体查询的状态。


## 用法

```jsx
import {useMedia} from 'react-use';

const Demo = () => {
  const isWide = useMedia('(min-width: 480px)');

  return (
    <div>
      Screen is wide: {isWide ? 'Yes' : 'No'}
    </div>
  );
};
```
