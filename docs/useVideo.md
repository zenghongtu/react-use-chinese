# `useVideo`

创建 `<video>` 元素，追踪其状态并暴露播放控件。


## 用法

```jsx
import {useVideo} from 'react-use';

const Demo = () => {
  const [video, state, controls, ref] = useVideo(
    <video src="http://clips.vorwaerts-gmbh.de/big_buck_bunny.mp4" autoPlay />
  );

  return (
    <div>
      {video}
      <pre>{JSON.stringify(state, null, 2)}</pre>
      <button onClick={controls.pause}>Pause</button>
      <button onClick={controls.play}>Play</button>
      <br/>
      <button onClick={controls.mute}>Mute</button>
      <button onClick={controls.unmute}>Un-mute</button>
      <br/>
      <button onClick={() => controls.volume(.1)}>Volume: 10%</button>
      <button onClick={() => controls.volume(.5)}>Volume: 50%</button>
      <button onClick={() => controls.volume(1)}>Volume: 100%</button>
      <br/>
      <button onClick={() => controls.seek(state.time - 5)}>-5 sec</button>
      <button onClick={() => controls.seek(state.time + 5)}>+5 sec</button>
    </div>
  );
};
```


## 参考

```jsx
const [video, state, controls, ref] = useVideo(props);
const [video, state, controls, ref] = useVideo(<video {...props}/>);
```

`video` 是 React 的 `<video>` 元素，你必须在渲染树中的某处插入，例如：

```jsx
<div>{video}</div>
```

`state` 追踪音频的状态，并具有以下状态：

```json
{
  "buffered": [
    {
      "start": 0,
      "end": 425.952625
    }
  ],
  "time": 5.244996,
  "duration": 425.952625,
  "isPlaying": false,
  "muted": false,
  "volume": 1
}
```

`controls` 是一个方法列表集合，运行你控制视频的播放，它有以下接口：

```ts
interface AudioControls {
  play: () => Promise<void> | void;
  pause: () => void;
  mute: () => void;
  unmute: () => void;
  volume: (volume: number) => void;
  seek: (time: number) => void;
}
```

`ref` 是对 HTML `<video>` 元素的 React 引用，你可以通过 `ref.current` 访问该元素，注意它可能是 `null`。

最后，`props` &mdash; `<video>` 接收所有的属性。
