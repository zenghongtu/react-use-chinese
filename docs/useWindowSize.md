# `useWindowSize`

React 传感器钩子，用于跟踪浏览器窗口的大小。


## 用法

```jsx
import {useWindowSize} from 'react-use';

const Demo = () => {
  const {width, height} = useWindowSize();

  return (
    <div>
      <div>width: {width}</div>
      <div>height: {height}</div>
    </div>
  );
};
```
