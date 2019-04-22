# `useScroll`

当 DOM 元素中的滚动位置发生更改时，React 传感器钩子将会重新渲染。

## Usage

```jsx
import {useScroll} from 'react-use';

const Demo = () => {
  const scrollRef = React.useRef(null);
  const {x, y} = useScroll(scrollRef);

  return (
    <div ref={scrollRef}>
      <div>x: {x}</div>
      <div>y: {y}</div>
    </div>
  );
};
```

## Reference

```ts
useScroll(ref: RefObject<HTMLElement>);
```
