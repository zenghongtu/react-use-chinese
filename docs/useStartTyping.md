# `useStartTyping`


React传感器钩子，用于在用户开始键入时触发回调。 可用于聚焦页面上的默认输入字段。

## Usage

```jsx
import useStartTyping from 'react-use/lib/useStartTyping';

const Demo = () => {
  useStartTyping(() => alert('Started typing...'));

  return null;
};
```
