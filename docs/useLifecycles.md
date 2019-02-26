# `useLifecycles`

当组件挂载和卸载时，React 生命周期钩子分别调用 `mount` 和 `unmount`  回调。

## 用法

```jsx
import {useLifecycles} from 'react-use';

const Demo = () => {
  useLifecycles(() => console.log('MOUNTED'), () => console.log('UNMOUNTED'));
  return null;
};
```


## 参考

```js
useLifecycles(mount, unmount);
```
