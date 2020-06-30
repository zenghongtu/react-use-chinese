# `useGetSetState`

`useGetSet` 和 `useSetState` 的混合。


## 用法

```jsx
import {useGetSetState} from 'react-use';

const Demo = () => {
  const [get, setState] = useGetSetState({cnt: 0});
  const onClick = () => {
    setTimeout(() => {
      setState({cnt: get().cnt + 1})
    }, 1_000);
  };

  return (
    <button onClick={onClick}>Clicked: {get().cnt}</button>
  );
};
```
