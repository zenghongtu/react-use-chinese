# `useOutsideClick`

React 用户界面钩子，当用户单击目标元素外部时触发回调。


## 用法

```jsx
import {useOutsideClick} from 'react-use';

const Demo = () => {
  const ref = useRef(null);
  useOutsideClick(ref, () => {
    console.log('OUTSIDE CLICKED');
  });

  return (
    <div ref={ref} style={{
      width: 200,
      height: 200,
      background: 'red',
    }} />
  );
};
```
