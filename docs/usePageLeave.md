# `usePageLeave`

当鼠标离开页面时，React 传感器钩子会触发回调。

## Usage

```jsx
import {usePageLeave} from 'react-use';

const Demo = () => {
  usePageLeave(() => console.log('Page left...'));

  return null;
};
```
