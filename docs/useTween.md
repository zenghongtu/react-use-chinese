# `useTween`

 React动画钩子，补间0到1之间的数字。

[![](https://img.shields.io/badge/demo-useTween-green.svg)](https://codesandbox.io/s/52990wwzyl)


## 用法

```jsx
import {useTween} from 'react-use';

const Demo = () => {
  const t = useTween();

  return (
    <div>
      Tween: {t}
    </div>
  );
};
```


## 参考

```ts
useTween(easing?: string, ms?: number, delay?: number): number
```

返回一个数字，该数字在动画结束时以0开始，以1结束。

- `easing` &mdash; 一个有效的 [easing names](https://github.com/streamich/ts-easing/blob/master/src/index.ts), 默认为 `inCirc`.
- `ms` &mdash; 保持重新渲染组件的时间, 默认为 `200`.
- `delay` &mdash; 延迟（以毫秒为单位），然后开始重新渲染组件, 默认为 `0`.
