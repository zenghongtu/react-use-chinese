# `useEffectOnce`

 React的生命周期钩子，只运行一次效果。

## Usage

```jsx
import {useEffectOnce} from 'react-use';

const Demo = () => {
  useEffectOnce(() => {
    console.log('Running effect once on mount')

    return () => {
      console.log('Running clean-up of effect on unmount')
    }
  });

  return null;
};
```

## Reference

```js
useEffectOnce(effect: EffectCallback);
```
