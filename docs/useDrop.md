# `useDrop` and `useDropArea`

触发文件，链接删除和复制粘贴。

`useDrop`跟踪整个页面的事件，`useDropArea`跟踪特定元素的拖放事件。


## Usage

`useDrop`:

```jsx
import {useDrop} from 'react-use';

const Demo = () => {
  const state = useDrop({
    onFiles: files => console.log('files', files),
    onUri: uri => console.log('uri', uri),
    onText: text => console.log('text', text),
  });

  return (
    <div>
      Drop something on the page.
    </div>
  );
};
```

`useDropArea`:

```jsx
import {useDropArea} from 'react-use';

const Demo = () => {
  const [bond, state] = useDropArea({
    onFiles: files => console.log('files', files),
    onUri: uri => console.log('uri', uri),
    onText: text => console.log('text', text),
  });

  return (
    <div {...bond}>
      Drop something here.
    </div>
  );
};
```
