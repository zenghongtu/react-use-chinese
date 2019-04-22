# `useKey`

当使用键盘键时，React UI 传感器钩子执行`handler`。

## Usage

```jsx
import useKey from 'react-use/lib/useKey';

const Demo = () => {
  const [count, set] = useState(0);
  const increment = () => set(count => ++count);
  useKey('ArrowUp', increment);

  return (
    <div>
      Press arrow up: {count}
    </div>
  );
};
```

Or as render-prop:

```jsx
import UseKey from 'react-use/lib/comps/UseKey';

<UseKey filter='a' fn={() => alert('"a" key pressed!')} />
```


## Reference

```js
useKey(filter, handler, options?, deps?)
```


## Examples

```js
useKey('a', () => alert('"a" pressed'));

const predicate = (event) => event.key === 'a'
useKey(predicate, handler, {event: 'keyup'});
```
