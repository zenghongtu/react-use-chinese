# `useLogger`

React lifecycle hook that logs in console as component transitions through life-cycles.

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
