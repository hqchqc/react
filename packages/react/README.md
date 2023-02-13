# `react`

<!-- React 是一个用于创建用户界面的 JavaScript 库 -->
React is a JavaScript library for creating user interfaces.

<!-- `react` 包仅包含定义 React 组件所需的功能。它通常与 React 渲染器一起使用，例如用于网络的“react-dom”或用于本地环境的“react-native” -->
The `react` package contains only the functionality necessary to define React components. It is typically used together with a React renderer like `react-dom` for the web, or `react-native` for the native environments.

<!-- 默认情况下，React 将处于开发模式。开发版本包括关于常见错误的额外警告，而生产版本包括额外的性能优化并删除所有错误消息。部署应用程序时，不要忘记使用[生产构建](https://reactjs.org/docs/optimizing-performance.html#use-the-production-build)。 -->
**Note:** by default, React will be in development mode. The development version includes extra warnings about common mistakes, whereas the production version includes extra performance optimizations and strips all error messages. Don't forget to use the [production build](https://reactjs.org/docs/optimizing-performance.html#use-the-production-build) when deploying your application.

## Usage

```js
import { useState } from 'react';
import { createRoot } from 'react-dom/client';

function Counter() {
  const [count, setCount] = useState(0);
  return (
    <>
      <h1>{count}</h1>
      <button onClick={() => setCount(count + 1)}>
        Increment
      </button>
    </>
  );
}

const root = createRoot(document.getElementById('root'));
root.render(<Counter />);
```

## Documentation

See https://reactjs.org/

## API

See https://reactjs.org/docs/react-api.html
