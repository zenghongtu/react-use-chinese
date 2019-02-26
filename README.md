<div align="center">
  <h1>
    <br/>
    <br/>
    👍
    <br />
    react-use
    <br />
    <br />
    <br />
    <br />
  </h1>
  <sup>
    <br />
    <br />
    <br />
    Collection of essential <a href="https://reactjs.org/docs/hooks-intro.html">React Hooks</a>.</em>
    <br />
    <em>Port of</em> <a href="https://github.com/streamich/libreact"><code>libreact</code></a>. <em>See <a href="http://streamich.github.io/react-use">demos</a>.</em>
  </sup>
  <br />
  <br />
  <br />
  <br />
  <pre>npm i <a href="https://www.npmjs.com/package/react-use">react-use</a></pre>
  <br />
  <br />
  <br />
  <br />
  <br />
</div>

- [**Sensors**](./docs/Sensors.md)
  - [`useBattery`](./docs/useBattery.md) &mdash; 跟踪设备电池状态。 [![][img-demo]](https://codesandbox.io/s/qlvn662zww)
  - [`useGeolocation`](./docs/useGeolocation.md) &mdash; 跟踪用户设备的地理位置状态。
  - [`useHover` and `useHoverDirty`](./docs/useHover.md) &mdash; 跟踪鼠标悬停某个元素的状态。 [![][img-demo]](https://codesandbox.io/s/zpn583rvx)
  - [`useIdle`](./docs/useIdle.md) &mdash; 跟踪用户是否处于非活动状态。
  - [`useKeyPress`](./docs/useKeyPress.md) &mdash; 跟踪是否按下了键盘键或一组键。
  - [`useLocation`](./docs/useLocation.md) &mdash; 跟踪页面导航栏的位置状态。
  - [`useMedia`](./docs/useMedia.md) &mdash; 跟踪CSS媒体查询的状态。
  - [`useMediaDevices`](./docs/useMediaDevices.md) &mdash; 跟踪连接的硬件设备的状态。
  - [`useMotion`](./docs/useMotion.md) &mdash; 跟踪设备的运动传感器的状态。
  - [`useNetwork`](./docs/useNetwork.md) &mdash; 跟踪用户的互联网连接状态。
  - [`useOrientation`](./docs/useOrientation.md) &mdash; 跟踪设备屏幕方向的状态。
  - [`useSize`](./docs/useSize.md) &mdash; 跟踪一些HTML元素的尺寸。
  - [`useWindowSize`](./docs/useWindowSize.md) &mdash;  跟踪 `Window` 大小. [![][img-demo]](https://codesandbox.io/s/m7ln22668)
    <br/>
    <br/>
  - [`useAudio`](./docs/useAudio.md) &mdash; 播放音频并公开其控件。 [![][img-demo]](https://codesandbox.io/s/2o4lo6rqy)
  - [`useOutsideClick`](./docs/useOutsideClick.md) &mdash; 当用户点击目标区域外时触发回调。
  - [`useSpeech`](./docs/useSpeech.md) &mdash; 从文本字符串合成语音。 [![][img-demo]](https://codesandbox.io/s/n090mqz69m)
  - [`useVideo`](./docs/useVideo.md) &mdash; 播放视频，跟踪其状态，以及公开播放控件。
  - [`useWait`](./docs/useWait.md) &mdash; UI的复杂等待管理。
    <br/>
    <br/>
- [**Animations**](./docs/Animations.md)
  - [`useRaf`](./docs/useRaf.md) &mdash; 在每个`requestAnimationFrame`上重新呈现组件。
  - [`useSpring`](./docs/useSpring.md) &mdash; 根据弹簧动力学随时间插入数字。
  - [`useTimeout`](./docs/useTimeout.md) &mdash; 超时后返回true。
  - [`useTween`](./docs/useTween.md) &mdash; 重新渲染组件，同时补间0到1之间的数字。 [![][img-demo]](https://codesandbox.io/s/52990wwzyl)
  - [`useUpdate`](./docs/useUpdate.md) &mdash; 返回一个回调，在调用时重新呈现组件。
    <br/>
    <br/>
- [**Side-effects**](./docs/Side-effects.md)
  - [`useAsync`](./docs/useAsync.md) &mdash; 解析异步函数。
  - [`useCss`](./docs/useCss.md) &mdash; 动态调整CSS。
  - [`useFavicon`](./docs/useFavicon.md) &mdash; 设置页面的favicon。
  - [`useLocalStorage`](./docs/useLocalStorage.md) &mdash; 管理`localStorage`中的值。
  - [`useSessionStorage`](./docs/useSessionStorage.md) &mdash; 管理`sessionStorage`中的值。
  - [`useTitle`](./docs/useTitle.md) &mdash; 设置页面标题。
  - [`useDebounce`](./docs/useDebounce.md) &mdash; 去抖函数。
    <br/>
    <br/>
- [**Lifecycles**](./docs/Lifecycles.md)
  - [`useLifecycles`](./docs/useLifecycles.md) &mdash; 调用`mount`和`unmount`回调。
  - [`useRefMounted`](./docs/useRefMounted.md) &mdash; 跟踪组件是否已挂载。
  - [`useLogger`](./docs/useLogger.md) &mdash; 在组件经历生命周期时登录控制台。
  - [`useMount`](./docs/useMount.md) &mdash; 调用`mount`回调。
  - [`useUnmount`](./docs/useUnmount.md) &mdash; 调用unmount回调。
    <br/>
    <br/>
- [**State**](./docs/State.md)
  - [`createMemo`](./docs/createMemo.md) &mdash; memoized hooks的工厂。
  - [`useCallbag`](./docs/useCallbag.md) &mdash; 跟踪callbag的最新值。
  - [`useGetSet`](./docs/useGetSet.md) &mdash; 返回状态getter `get()`而不是raw状态。
  - [`useGetSetState`](./docs/useGetSetState.md) &mdash; 就像`useGetSet`和`useSetState`有一个孩子。
  - [`useObservable`](./docs/useObservable.md) &mdash; 跟踪`Observable`的最新值。
  - [`useSetState`](./docs/useSetState.md) &mdash; 创建类似`this.setState`的`setState`方法。[![][img-demo]](https://codesandbox.io/s/n75zqn1xp0)
  - [`useToggle` and `useBoolean`](./docs/useToggle.md) &mdash; 跟踪布尔值的状态。
  - [`useCounter` and `useNumber`](./docs/useCounter.md) &mdash; 跟踪数字的状态。
  - [`useList`](./docs/useList.md) &mdash; 跟踪数组的状态。
  - [`useMap`](./docs/useMap.md) &mdash; 跟踪对象的状态。
    <br/>
    <br/>

<br />
<br />
<br />

<h2 align="center"><sub>使用</sub></h2>

<br/>

<p align="center">
要使用Hooks API，你需要安装React <code>16.8.1</code> 或更高版本。
</p>

<p align="center">
你可以单独导入每个钩子 <code>import useToggle from 'react-use/lib/useToggle'</code>.
</p>

<br/>

<h2 align="center"><sub>许可证</sub></h2>

<p align="center">
  <a href="./LICENSE">Unlicense</a> &mdash; 公有领域
</p>

[img-demo]: https://img.shields.io/badge/demo-%20%20%20%F0%9F%9A%80-green.svg
