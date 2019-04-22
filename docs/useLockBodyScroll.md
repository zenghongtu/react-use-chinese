# `useLockBodyScroll`

React side-effect hook that locks scrolling on the body element. Useful for modal and other overlay components.

React 锁定在 body 元素上滚动的副作用钩子。适用于模态框和其他覆盖层组件。


## Usage

```jsx
import {useLockBodyScroll, useToggle} from 'react-use';

const Demo = () => {
  const [locked, toggleLocked] = useToggle(false)

  useLockBodyScroll(locked);

  return (
    <div>
      <button onClick={() => toggleLocked()}>
        {locked ? 'Unlock' : 'Lock'}
      </button>
    </div>
  );
};
```

## Reference

```ts
useLockBodyScroll(enabled?: boolean = true);
```

- `enabled` &mdash; Hook will lock scrolling on the body element if `true`, defaults to `true`
