# `useMount`

React lifecycle hook that call `mount` callback, when
component is mounted.


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
