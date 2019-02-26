# `useUpdate`

 React实用程序钩子，它返回一个强制组件在被调用时重新呈现的函数。


## 用法

```jsx
import {useUpdate} from 'react-use';

const Demo = () => {
  const update = useUpdate();
  return (
    <>
      <div>Time: {Date.now()}</div>
      <button onClick={update}>Update</button>
    </>
  );
};
```
