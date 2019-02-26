# `useCallbag`

React 状态钩子，用于追踪 callbag 最新值。


## 用法

```jsx
import {useCallbag} from 'react-use';
import interval from 'callbag-interval';

const Demo = () => {
  const count = useCallbag(() => interval(1000));
  return <span>{`Counter: ${count}`}</span>
};
```
