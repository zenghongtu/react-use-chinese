# `useLocalStorage`

React 副作用钩子，用于管理单个 `localStorage` 键。


## 用法

```jsx
import {useLocalStorage} from 'react-use';

const Demo = () => {
  const [value, setValue] = useLocalStorage('my-key', 'foo');

  return (
    <div>
      <div>Value: {value}</div>
      <button onClick={() => setValue('bar')}>bar</button>
      <button onClick={() => setValue('baz')}>baz</button>
    </div>
  );
};
```


## 参考

```js
useLocalStorage(key);
useLocalStorage(key, initialValue);
useLocalStorage(key, initialValue, raw);
```

- `key` &mdash; `localStorage` 键来管理。
- `initialValue` &mdash; 要设置的初始化值，如果`localStorage`中的值为空。
- `raw` &mdash; boolean，如果设为 true，钩子将不会尝试 JSON 序列化存储的值。
