# `useWindowScroll`

React 传感器钩子，在窗口滚动时重新渲染。

## Usage

```jsx
import {useWindowScroll} from 'react-use';

const Demo = () => {
  const {x, y} = useWindowScroll();

  return (
    <div>
      <div>x: {x}</div>
      <div>y: {y}</div>
    </div>
  );
};
```
