# `useKeyboardJs`

React UI传感器钩子，可检测复杂的键组合，如检测时间

多个键同时按下或要求按指定的顺序按下它们。

通过[KeyboardJS键组合]（https://github.com/RobertWHurst/KeyboardJS）。

有关如何制作组合字符串的更多详细信息，请查看其文档。

## Usage

```jsx
import useKeyboardJs from 'react-use/lib/useKeyboardJs';

const Demo = () => {
  const [isPressed] = useKeyboardJs('a + b');

  return (
    <div>
      [a + b] pressed: {isPressed ? 'Yes' : 'No'}
    </div>
  );
};
```

## Requirements

Install [`keyboardjs`](https://github.com/RobertWHurst/KeyboardJS) peer dependency:

```bash
npm add keyboardjs
# or
yarn add keyboardjs
```

## Reference

```js
useKeyboardJs(combination: string): [isPressed: boolean, event?: KeyboardEvent]
```
