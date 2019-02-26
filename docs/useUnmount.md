# `useUnmount`

React lifecycle hook that call `unmount` callback, when
component is un-mounted.


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
