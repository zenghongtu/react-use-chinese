# `useOrientation`

React 传感器钩子，跟踪用户设备的屏幕方向。

以以下形式返回状态：

```js
{
  angle: 0,
  type: 'landscape-primary'
}
```


## 用法

```jsx
import {useOrientation} from 'react-use';

const Demo = () => {
  const state = useOrientation();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
