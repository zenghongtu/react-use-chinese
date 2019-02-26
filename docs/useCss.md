# `useCss`

React 副作用钩子，用于 [CSS 动态][gen-5] 改变。

## 用法

```jsx
import {useCss} from 'react-use';

const Demo = () => {
  const className = useCss({
    color: 'red',
    border: '1px solid red',
    '&:hover': {
      color: 'blue',
    },
  });

  return (
    <div className={className}>
      Hover me!
    </div>
  );
};
```

[gen-5]: https://github.com/streamich/freestyler/blob/master/docs/en/generations.md#5th-generation
