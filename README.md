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
    <a href="https://www.npmjs.com/package/react-use">
      <img src="https://img.shields.io/npm/v/react-use.svg" alt="npm package" />
    </a>
    <a href="https://circleci.com/gh/streamich/react-use">
      <img src="https://img.shields.io/circleci/project/github/streamich/react-use/master.svg" alt="CircleCI master" />
    </a>
    <a href="https://www.npmjs.com/package/react-use">
      <img src="https://img.shields.io/npm/dm/react-use.svg" alt="npm downloads" />
    </a>
    <a href="http://streamich.github.io/react-use">
      <img src="https://img.shields.io/badge/demos-🚀-yellow.svg" alt="demos" />
    </a>
    <br />
    必不可少的 <a href="https://reactjs.org/docs/hooks-intro.html">React Hooks</a>集合.</em>
     <a href="https://github.com/streamich/libreact"><code>libreact</code></a><em>的港口</em>.
    <br />
    原仓库: <a href="https://github.com/streamich/react-use">react-use</a> v8.1.3
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

- [**传感器**](./docs/Sensors.md)
  - [`useBattery`](./docs/useBattery.md) &mdash; 跟踪设备电池状态。 [![][img-demo]](https://codesandbox.io/s/qlvn662zww)
  - [`useGeolocation`](./docs/useGeolocation.md) &mdash; 跟踪用户设备的地理位置状态。 [![][img-demo]](https://streamich.github.io/react-use/?path=/story/sensors-usegeolocation--demo)
  - [`useHover` and `useHoverDirty`](./docs/useHover.md) &mdash; 跟踪鼠标悬停某个元素的状态。 [![][img-demo]](https://codesandbox.io/s/zpn583rvx)
  - [`useIdle`](./docs/useIdle.md) &mdash; 跟踪用户是否处于非活动状态。
  - [`useKey`](./docs/useKey.md), [`useKeyPress`](./docs/useKeyPress.md), [`useKeyboardJs`](./docs/useKeyboardJs.md), 和 [`useKeyPressEvent`](./docs/useKeyPressEvent.md) &mdash; 追踪按键。 [![][img-demo]](https://streamich.github.io/react-use/?path=/story/sensors-usekeypressevent--demo)
  - [`useLocation`](./docs/useLocation.md) &mdash; 跟踪页面导航栏的位置状态。
  - [`useMedia`](./docs/useMedia.md) &mdash; 跟踪CSS媒体查询的状态。 [![][img-demo]](https://streamich.github.io/react-use/?path=/story/sensors-usemedia--demo)
  - [`useMediaDevices`](./docs/useMediaDevices.md) &mdash; 跟踪连接的硬件设备的状态。
  - [`useMotion`](./docs/useMotion.md) &mdash; 跟踪设备的运动传感器的状态。
  - [`useMouse` and `useMouseHovered`](./docs/useMouse.md) &mdash; 跟踪鼠标位置的状态。 [![][img-demo]](https://streamich.github.io/react-use/?path=/story/sensors-usemouse--docs)
  - [`useNetwork`](./docs/useNetwork.md) &mdash; 跟踪用户的互联网连接状态。
  - [`useOrientation`](./docs/useOrientation.md) &mdash; 跟踪设备屏幕方向的状态。
  - [`usePageLeave`](./docs/usePageLeave.md) &mdash; 当鼠标离开页面边界时触发。
  - [`useScroll`](./docs/useScroll.md) &mdash; 跟踪HTML元素的滚动位置。 [![][img-demo]](https://streamich.github.io/react-use/?path=/story/sensors-usescroll--docs)
  - [`useSize`](./docs/useSize.md) &mdash; 跟踪HTML元素的维度。
  - [`useStartTyping`](./docs/useStartTyping.md) &mdash; 检测用户何时开始输入。
  - [`useWindowScroll`](./docs/useWindowScroll.md) &mdash; 跟踪 `窗口` 滚动位置。 [![][img-demo]](https://streamich.github.io/react-use/?path=/story/sensors-usewindowscroll--docs)
  - [`useWindowSize`](./docs/useWindowSize.md) &mdash; 跟踪 `窗口` 尺寸。 [![][img-demo]](https://codesandbox.io/s/m7ln22668)
    <br/>
    <br/>
- [**用户界面**](./docs/UI.md)
  - [`useAudio`](./docs/useAudio.md) &mdash; 播放音频并公开其控件。 [![][img-demo]](https://codesandbox.io/s/2o4lo6rqy)
  - [`useClickAway`](./docs/useClickAway.md) &mdash; 当用户点击目标区域外时触发回调。
  - [`useCss`](./docs/useCss.md) &mdash; 动态调整CSS。
  - [`useDrop` and `useDropArea`](./docs/useDrop.md) &mdash; 跟踪文件，链接和复制粘贴。
  - [`useFullscreen`](./docs/useFullscreen.md) &mdash; 全屏显示元素或视频。 [![][img-demo]](https://streamich.github.io/react-use/?path=/story/ui-usefullscreen--demo)
  - [`useSpeech`](./docs/useSpeech.md) &mdash; 从文本字符串合成语音。 [![][img-demo]](https://codesandbox.io/s/n090mqz69m)
  - [`useVideo`](./docs/useVideo.md) &mdash; 播放视频，跟踪其状态，以及公开播放控件。 [![][img-demo]](https://streamich.github.io/react-use/?path=/story/ui-usevideo--demo)
  - [`useWait`](./docs/useWait.md) &mdash; UI的复杂等待管理。
    <br/>
    <br/>
- [**动画效果**](./docs/Animations.md)
  - [`useRaf`](./docs/useRaf.md) &mdash; 在每个 `requestAnimationFrame` 上重新呈现组件。
  - [`useSpring`](./docs/useSpring.md) &mdash; 根据弹簧动力学随时间插入数字。
  - [`useTimeout`](./docs/useTimeout.md) &mdash; 超时后返回true。
  - [`useTween`](./docs/useTween.md) &mdash; 重新渲染组件，同时补间0到1之间的数字。 [![][img-demo]](https://codesandbox.io/s/52990wwzyl)
  - [`useUpdate`](./docs/useUpdate.md) &mdash; 返回一个回调，在调用时重新呈现组件。
    <br/>
    <br/>
- [**副作用**](./docs/Side-effects.md)
  - [`useAsync`](./docs/useAsync.md) &mdash; 解析一个 `async` 函数。
  - [`useAsyncFn`](./docs/useAsyncFn.md) &mdash; 异步函数的状态管理。
  - [`useAsyncRetry`](./docs/useAsyncRetry.md) &mdash; `useAsync` 带有 `retry()`方法。
  - [`useBeforeUnload`](./docs/useBeforeUnload.md) &mdash; 当用户尝试重新加载或关闭页面时显示浏览器警报。
  - [`useCopyToClipboard`](./docs/useCopyToClipboard.md) &mdash; 将文本复制到剪贴板。
  - [`useDebounce`](./docs/useDebounce.md) &mdash; 防抖函数。 [![][img-demo]](https://streamich.github.io/react-use/?path=/story/side-effects-usedebounce--demo)
  - [`useFavicon`](./docs/useFavicon.md) &mdash; 设置页面的favicon。
  - [`useLocalStorage`](./docs/useLocalStorage.md) &mdash; 管理`localStorage`中的值。
  - [`useLockBodyScroll`](./docs/useLockBodyScroll.md) &mdash; 锁定body元素的滚动。
  - [`useSessionStorage`](./docs/useSessionStorage.md) &mdash; 管理`sessionStorage`中的值。
  - [`useThrottle` and `useThrottleFn`](./docs/useThrottle.md) &mdash; 节流一个函数。[![][img-demo]](https://streamich.github.io/react-use/?path=/story/side-effects-usethrottle--demo)
  - [`useTitle`](./docs/useTitle.md) &mdash; 设置页面标题。
    <br/>
    <br/>
- [**生命周期**](./docs/Lifecycles.md)
  - [`useEffectOnce`](./docs/useEffectOnce.md) &mdash; 仅运行一次的修改后的[`useEffect`](https://reactjs.org/docs/hooks-reference.html#useeffect)。
  - [`useEvent`](./docs/useEvent.md) &mdash; 订阅事件。
  - [`useLifecycles`](./docs/useLifecycles.md) &mdash; 调用`mount`和`unmount`回调。
  - [`useRefMounted`](./docs/useRefMounted.md) &mdash; 跟踪组件是否已挂载。
  - [`usePromise`](./docs/usePromise.md) &mdash; 仅在安装组件时解析promise。
  - [`useLogger`](./docs/useLogger.md) &mdash; 在组件经历生命周期时登录控制台。
  - [`useMount`](./docs/useMount.md) &mdash; 调用`mount`回调。
  - [`useUnmount`](./docs/useUnmount.md) &mdash; 调用`unmount`回调。
  - [`useUpdateEffect`](./docs/useUpdateEffect.md) &mdash; 仅在更新时运行一个`effect`。
  - [`useDeepCompareEffect`](./docs/useDeepCompareEffect.md) &mdash; 运行一个`effect`通过深度比较其依赖项。
    <br/>
    <br/>
- [**状态**](./docs/State.md)
  - [`createMemo`](./docs/createMemo.md) &mdash; memoized hooks的工厂钩子。
  - [`useGetSet`](./docs/useGetSet.md) &mdash; 返回状态 getter `get()` 而不是原始状态。
  - [`useGetSetState`](./docs/useGetSetState.md) &mdash; 就像 [`useGetSet`](./docs/useGetSet.md) 和 [`useSetState`](./docs/useSetState.md) 有个孩子。
  - [`useObservable`](./docs/useObservable.md) &mdash; 跟踪`Observable`的最新值。
  - [`useSetState`](./docs/useSetState.md) &mdash; 创建类似`this.setState`的`setState`方法。[![][img-demo]](https://codesandbox.io/s/n75zqn1xp0)
  - [`useToggle` and `useBoolean`](./docs/useToggle.md) &mdash; 跟踪布尔值的状态。
  - [`useCounter` and `useNumber`](./docs/useCounter.md) &mdash; 跟踪数字的状态。
  - [`useList`](./docs/useList.md) &mdash; 跟踪数组的状态。
  - [`useMap`](./docs/useMap.md) &mdash; 跟踪对象的状态。

## Usage

你需要安装React [`16.8.0`](https://reactjs.org/blog/2019/02/06/react-v16.8.0.html)或更高版本才能使用Hooks API。你可以分别导入每个钩子

```js
import useToggle from 'react-use/lib/useToggle'
```

或使用 ES6 命名导入

```js
import {useToggle} from 'react-use'
```

根据绑定器的不同，你可能会在ES6命名导入语句中遇到缺少依赖项的错误。有些钩子要求安装对等依赖项，因此我们建议单独导入。如果你希望同时使用这两种方法，你可以通过将以下配置添加到`.babelrc`文件中，将命名的导入语句转换为使用[`babel-plugin-import`](https://github.com/ant-design/babel-plugin-import)的单个导入语句。

```json
[
  "import", {
    "libraryName": "react-use",
    "libraryDirectory": "lib",
    "camel2DashComponentName": false
  }
]
```

<h2 align="center"><sub>许可证</sub></h2>

<p align="center">
  <a href="./LICENSE">Unlicense</a> &mdash; 公有领域
</p>

[img-demo]: https://img.shields.io/badge/demo-%20%20%20%F0%9F%9A%80-green.svg
