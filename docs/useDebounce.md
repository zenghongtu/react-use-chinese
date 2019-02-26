# `useDebounce`

React 钩子，会延迟调用函数，直到上次调用防抖函数以后经过等待毫秒之后。

第三个参数是防抖所依赖的数组值，其方式与 useEffect 中的相同。当其中一个值发生改变，防抖超时将会启动。

## 用法

```jsx
import React, { useState } from 'react';
import { useDebounce } from 'react-use';

const Demo = () => {
  const [state, setState] = React.useState('Typing stopped');
  const [val, setVal] = React.useState('');

  useDebounce(
    () => {
      setState('Typing stopped');
    },
    2000,
    [val]
  );

  return (
    <div>
      <input
        type="text"
        value={val}
        placeholder="Debounced input"
        onChange={({ currentTarget }) => {
          setState('Waiting for typing to stop...');
          setVal(currentTarget.value);
        }}
      />
      <div>{state}</div>
    </div>
  );
};
```

## 参考

```ts
useDebouce(fn, ms: number, args: any[]);
```
