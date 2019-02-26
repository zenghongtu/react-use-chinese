# `useMotion`

React sensor hook that uses device's acceleration sensor to track its motions.


## 用法

```jsx
import {useMotion} from 'react-use';

const Demo = () => {
  const state = useMotion();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
