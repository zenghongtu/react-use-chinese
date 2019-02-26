# `useSpring`

React 动画钩子，根据弹簧动力学随时间更新单个数值。

## 用法

```jsx
import {useSpring} from 'react-use';

const Demo = () => {
  const [target, setTarget] = useState(50);
  const value = useSpring(target);

  return (
    <div>
      {value}
      <br />
      <button onClick={() => setTarget(0)}>Set 0</button>
      <button onClick={() => setTarget(100)}>Set 100</button>
    </div>
  );
};
```


# 参考


```js
const currentValue = useSpring(targetValue);
const currentValue = useSpring(targetValue, tension, friction);
```
