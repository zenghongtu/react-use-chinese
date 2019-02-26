# `useUnmount`

当组件被卸载时，调用 `unmount` 回调的生命周期钩子。


## 用法

```jsx
import {useUnmount} from 'react-use';

const Demo = () => {
  useUnmount(() => console.log('UNMOUNTED'));
  return null;
};
```


## 参考

```js
useUnmount(mount);
```
