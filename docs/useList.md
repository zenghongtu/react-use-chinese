# `useList`

React state hook that tracks a value of an array.


## 用法

```jsx
import {useList} from 'react-use';

const Demo = () => {
  const [list, {set, push}] = useList();

  return (
    <div>
      <div>{list.join(',')}</div>
      <button onClick={() => set([])}>Reset</button>
      <button onClick={() => push(Date.now())}>Push</button>
    </div>
  );
};
```
