# `useSpeech`

React 用户界面钩子，用于合成说出给定字符串的人声。

[![](https://img.shields.io/badge/demo-useSpeech-green.svg)](https://codesandbox.io/s/n090mqz69m)


## 用法

```jsx
import {useSpeech} from 'react-use';

const Demo = () => {
  const state = useSpeech('Hello world!');

  return (
    <pre>
      {JSON.stringify(state, null, 2)}
    </pre>  
  );
};
```
