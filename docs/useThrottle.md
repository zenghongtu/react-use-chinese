# `useThrottle` and `useThrottleFn`

用于节流的 React 钩子。

## Usage

```jsx
import React, { useState } from 'react';
import { useThrottle, useThrottleFn } from 'react-use';

const Demo = ({value}) => {
  const throttledValue = useThrottle(value);
  // const throttledValue = useThrottleFn(value => value, 200, [value]);

  return (
    <>
      <div>Value: {value}</div>
      <div>Throttled value: {throttledValue}</div>
    </>
  );
};
```

## Reference

```ts
useThrottle(value, ms?: number);
useThrottleFn(fn, ms, args);
```
