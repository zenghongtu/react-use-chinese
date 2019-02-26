# `useLogger`

React生命周期钩子，在生命周期中作为组件转换记录到控制台。

## 用法

```jsx
import {useLogger} from 'react-use';

const Demo = (props) => {
  useLogger('Demo', props);
  return null;
};
```


## Example Output

```
Demo mounted
Demo props updated {}
Demo un-mounted
```


## 参考

```js
useLogger(name, props);
```

- `name` &mdash; component name.
- `props` &mdash; latest props.
