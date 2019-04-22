# `useDeepCompareEffect`

一个修改的 useEffect 钩子，它使用对其依赖项的深度比较而不是引用的相等性。

## Usage

```jsx
import {useCounter, useDeepCompareEffect} from 'react-use';

const Demo = () => {
  const [count, {inc: inc}] = useCounter(0);
  const options = { step: 2 };

  useDeepCompareEffect(() => {
    inc(options.step)
  }, [options]);

  return (
    <div>
      <p>useDeepCompareEffect: {count}</p>
    </div>
  );
};
```

## Reference

```ts
useDeepCompareEffect(effect: () => void | (() => void | undefined), deps: any[]);
```
