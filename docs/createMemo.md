# `createMemo`

钩子（Hook）工厂，接收一个要被记忆的函数，返回一个带有记忆功能的 React 钩子，该钩子接收到相同的参数时返回和原始函数相同的结果。


## 用法

```jsx
import {createMemo} from 'react-use';

const fibonacci = n => {
  if (n === 0) return 1;
  if (n === 1) return 2;
  return fibonacci(n - 1) + fibonacci(n - 2);
};

const useMemoFibonacci = createMemo(fibonacci);

const Demo = () => {
  const result = useMemoFibonacci(10);

  return (
    <div>
      fib(10) = {result}
    </div>
  );
};
```


## 参考

```js
const useMemoFn = createMemo(fn);
```
