# `useHover` and `useHoverDirty`

React 用户界面传感器钩子，用于追踪某个元素是否有鼠标悬停。

- `useHover` 接收一个 React 元素或者返回一个元素的函数，`useHoverDirty` 接收 React ref。
- `useHover` 设置 react `onMouseEnter` 和 `onMouseLeave` 事件,
`useHoverDirty` 设置 DOM `onmouseover` 和 `onmouseout` 事件.

## 用法

```jsx
import {useHover} from 'react-use';

const Demo = () => {
  const element = (hovered) =>
    <div>
      Hover me! {hovered && 'Thanks!'}
    </div>;
  const [hoverable, hovered] = useHover(element);

  return (
    <div>
      {hoverable}
      <div>{hovered ? 'HOVERED' : ''}</div>
    </div>
  );
};
```


## 参考

```js
const [newReactElement, isHovering] = useHover(reactElement);
const [newReactElement, isHovering] = useHover((isHovering) => reactElement);
const isHovering = useHoverDirty(ref);
```
