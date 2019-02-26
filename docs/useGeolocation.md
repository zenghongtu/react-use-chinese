# `useGeolocation`

React sensor hook that tracks user's geographic location.


## 用法

```jsx
import {useGeolocation} from 'react-use';

const Demo = () => {
  const state = useGeolocation();

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>
  );
};
```
