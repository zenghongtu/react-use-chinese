# `useClickAway`

当用户在目标元素外部单击时，React UI 钩子触发回调。


## Usage

```jsx
import {useClickAway} from 'react-use';

const Demo = () => {
  const ref = useRef(null);
  useClickAway(ref, () => {
    alert('OUTSIDE CLICKED');
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
