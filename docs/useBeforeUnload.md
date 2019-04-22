# `useBeforeUnload`

React 副作用钩子，当用户试图重新加载或关闭页面时显示浏览器警报。

## Usage

```jsx
import {useBeforeUnload} from 'react-use';

const Demo = () => {
  const [dirty, toggleDirty] = useToggle(false);
  useBeforeUnload(dirty, 'You have unsaved changes, are you sure?');

  return (
    <div>
      {dirty && <p>Try to reload or close tab</p>}
      <button onClick={() => toggleDirty()}>{dirty ? 'Disable' : 'Enable'}</button>
    </div>
  );
};
```
