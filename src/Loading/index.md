---
nav:
  path: /components
  order: 2
  title: 组件
---

## Loading

Demo:

```tsx
import React from 'react';
import {Button} from "antd"
import { Loading } from 'library-template';

export default () => {
  function showGlobalLoading() {
    Loading.global(true);

    setTimeout(() => {
      Loading.global(false)
    }, 3000)
  }

  return (
    <>
      <Button onClick={showGlobalLoading}>全局Loading</Button>
    </>
  )
};
```

More skills for writing demo: https://d.umijs.org/guide/demo-principle
