# `usePromise`

React Lifecycle钩子，它返回一个包装promises的辅助函数。

使用此函数包装的 Promises 将仅在安装组件时进行解析。

## Usage

```jsx
import {usePromise} from 'react-use';

const Demo = ({promise}) => {
  const mounted = usePromise();
  const [value, setValue] = useState();

  useEffect(() => {
    (async () => {
      const value = await mounted(promise);
      // This line will not execute if <Demo> component gets unmounted.
      setValue(value);
    })();
  });
};
```
