# `useRaf`

 React动画钩子,强制组件在每个 `reaquestAnimationFrame` 上重新渲染，返回经过的时间百分比。


## 用法

```jsx
import {useRaf} from 'react-use';

const Demo = () => {
  const elapsed = useRaf(5000, 1000);

  return (
    <div>
      Elapsed: {elapsed}
    </div>
  );
};
```


## 参考

```ts
useRaf(ms?: number, delay?: number): number;
```

- `ms` &mdash; milliseconds  保持重新渲染组件的时间, 默认为 `1e12`.
- `delay` &mdash; 延迟（以毫秒为单位），然后开始重新渲染组件, 默认为 `0`.
