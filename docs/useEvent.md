# `useEvent`

 React传感器钩子，它为事件订阅`handler`。

## Usage

```jsx
import useEvent from 'react-use/lib/useEvent';
import useList from 'react-use/lib/useList';

const Demo = () => {
  const [list, {push, clear}] = useList();

  const onKeyDown = useCallback(({key}) => {
    if (key === 'r') clear();
    push(key);
  }, []);

  useEvent('keydown', onKeyDown);

  return (
    <div>
      <p>
        Press some keys on your keyboard, <code style={{color: 'tomato'}}>r</code> key resets the list
      </p>
      <pre>
        {JSON.stringify(list, null, 4)}
      </pre>
    </div>
  );
};
```


## Examples

```js
useEvent('keydown', handler)
useEvent('scroll', handler, window, {capture: true})
```
