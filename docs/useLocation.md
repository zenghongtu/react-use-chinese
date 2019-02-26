# `useLocation`

React 传感器钩子，用于追踪浏览器的位置。

对于 Internet Explorer，你需要安装[polyfill](https://github.com/streamich/react-use/issues/73)。


## 用法

```jsx
import {useLocation} from 'react-use';

const Demo = () => {
  const state = useLocation();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
