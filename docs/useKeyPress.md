# `useKeyPress`

React 用户界面传感器钩子，用于检测用户何时按下键盘上的特殊键。

通过[KeyboardJS key combos](https://github.com/RobertWHurst/KeyboardJS)可以使用复杂的绑定，如检测何时同时按住多个建或要求他们按照指定的顺序按住它们。有关如何创建组合字符串的更多详细内容，请查阅其文档。

## 用法

```jsx
import { useKeyPress } from "react-use";

const Demo = () => {
  const hasPressedQ = useKeyPress("q");
  const hasPressedW = useKeyPress("w");
  const hasPressedE = useKeyPress("e");
  const hasPressedR = useKeyPress("r");
  const hasPressedT = useKeyPress("t");
  const hasPressedY = useKeyPress("y");
  const hasPressedWord = useKeyPress("q + w + e + r + t + y", {
    useKeyboardJS: true
  });

  return (
    <div>
      Try pressing each one of these at a time: <code>Q W E R T Y</code>
      {!hasPressedWord && (
        <div>
          {hasPressedQ && "Q"}
          {hasPressedW && "W"}
          {hasPressedE && "E"}
          {hasPressedR && "R"}
          {hasPressedT && "T"}
          {hasPressedY && "Y"}
        </div>
      )}
      <div>And now press them all at once!</div>
      <div>{hasPressedWord && "Q + W + E + R + T + Y"}</div>
    </div>
  );
};
```

## 参考

```js
const hasPressedSingleKey = useKeyPress("<key>");
const hasPressedKeyCombo = useKeyPress("<key combo>", {
  useKeyboardJS: true
});
```
