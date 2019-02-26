# `useSetState`

React 状态钩子，用于创建和 `this.setState` 在类组件中作用相似的 `setState` 方法--它将更改的对象合并到当前状态中。


## 用法

```jsx
import {useSetState} from 'react-use';

const Demo = () => {
  const [state, setState] = useSetState({});

  return (
    <div>
      <pre>{JSON.stringify(state, null, 2)}</pre>
      <button onClick={() => setState({hello: 'world'})}>hello</button>
      <button onClick={() => setState({foo: 'bar'})}>foo</button>
      <button 
        onClick={() => {
          setState((prevState) => ({
            count: (prevState.count || 0) + 1,
          }))
        }}
      >
        count
      </button>
    </div>
  );
};
```

## 参考

```js
const [state, setState] = useSetState({cnt: 0});

setState({cnt: state.cnt + 1});
setState((prevState) => ({
  cnt: prevState + 1,
}));
```
