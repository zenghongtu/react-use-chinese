# `useThrottleFn`

React hook that invokes a function and then delays subsequent function calls until after wait milliseconds have elapsed since the last time the throttled function was invoked.

The third argument is the array of values that the throttle depends on, in the same manner as useEffect. The throttle timeout will start when one of the values changes.

React 钩子，它调用一个函数然后延迟后续函数调用，直到自上次调用了受限制函数后经过等待的毫秒数。

第三个参数是节流所依赖的值，是一个数组，与useEffect的方式相同。 当其中一个值发生变化时，将会开始节流超时。

## Usage

```jsx
import React, { useState } from 'react';
import { useThrottleFn } from 'react-use';

const Demo = () => {
  const [status, setStatus] = React.useState('Updating stopped');
  const [value, setValue] = React.useState('');
  const [throttledValue, setThrottledValue] = React.useState('');

  useThrottleFn(
    () => {
      setStatus('Waiting for input...');
      setThrottledValue(value);
    },
    2000,
    [value]
  );

  return (
    <div>
      <input
        type="text"
        value={value}
        placeholder="Throttled input"
        onChange={({ currentTarget }) => {
          setStatus('Updating stopped');
          setValue(currentTarget.value);
        }}
      />
      <div>{status}</div>
      <div>Throttled value: {throttledValue}</div>
    </div>
  );
};
```

## Reference

```ts
useThrottleFn(fn, ms: number, args: any[]);
```
