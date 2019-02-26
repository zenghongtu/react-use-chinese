# `useLifecycles`

React lifecycle hook that call `mount` and `unmount` callbacks, when
component is mounted and un-mounted, respectively.


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
