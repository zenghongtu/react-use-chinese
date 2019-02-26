# `useRefMounted`

Lifecycle hook that tracks if component is mounted. Returns a ref, which has a
boolean `.current` property.


## 用法

```jsx
import {useRefMounted} from 'react-use';

const Demo = () => {
  const refMounted = useRefMounted();

  useEffect(() => {
    setTimeout(() => {
      if (refMounted.currrent) {
        // ...
      } else {
        // ...
      }
    }, 1000);
  });
};
```
