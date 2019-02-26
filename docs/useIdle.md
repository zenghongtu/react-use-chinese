# `useIdle`

React sensor hook that tracks if user on the page is idle.


## 用法

```jsx
import {useIdle} from 'react-use';

const Demo = () => {
  const isIdle = useIdle(3e3);

  return (
    <div>
      <div>User is idle: {isIdle ? 'Yes 😴' : 'Nope'}</div>
    </div>
  );
};
```


## 参考

```js
useIdle(ms, initialState);
```

- `ms` &mdash; time in milliseconds after which to consider use idle, defaults to `60e3` &mdash; one minute.
- `initialState` &mdash; whether to consider user initially idle, defaults to false.
