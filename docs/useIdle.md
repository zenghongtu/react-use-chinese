# `useIdle`

React 状态钩子，用于追踪页面上的用户是否空闲。

## 用法

```jsx
import {useIdle} from 'react-use';

const Demo = () => {
  const isIdle = useIdle(3e3);

  return (
    <div>
      <div>User is idle: {isIdle ? 'Yes 😴' : 'Nope'}</div>
    </div>
  );
};
```


## 参考

```js
useIdle(ms, initialState);
```

- `ms` &mdash; 考虑使用空闲时间的毫秒时间, 默认为 `60e3` &mdash; 1分钟。
- `initialState` &mdash; 是否考虑用户初始空闲，默认为 false。
