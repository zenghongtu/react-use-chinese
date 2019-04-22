# `useMouse` and `useMouseHovered`

React 感器钩子，在鼠标位置更改时重新渲染。 `useMouse`只是跟踪鼠标位置; `useMouseHovered`允许你指定额外的选项：

- `bound` &mdash; 绑定元素中的鼠标坐标

- `whenHovered` &mdash; 是否仅当用户将鼠标悬停在元素上时才附加`mousemove`事件处理程序

## Usage

```jsx
import {useMouse} from 'react-use';

const Demo = () => {
  const ref = React.useRef(null);
  const {docX, docY, posX, posY, elX, elY, elW, elH} = useMouse(ref);

  return (
    <div ref={element}>
      <div>Mouse position in document - x:{docX} y:{docY}</div>
      <div>Mouse position in element - x:{posX} y:{posY}</div>
      <div>Element position - x:{elX} y:{elY}</div>
      <div>Element dimensions - {elW}x{elH}</div>
    </div>
  );
};
```

## Reference

```ts
useMouse(ref);
useMouseHovered(ref, {bound: false, whenHovered: false});
```
