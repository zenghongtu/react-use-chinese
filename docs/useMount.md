# `useMount`

当组件被挂载时，响应调用 `mount` 回调的生命周期钩子。


## 用法

```jsx
import {useMount} from 'react-use';

const Demo = () => {
  useMount(() => console.log('MOUNTED'));
  return null;
};
```


## 参考

```js
useMount(mount);
```
