使用preload资源提示异步加载CSS文件

```html
<link rel="preload" href="xxx.css" as="style" onload="this.ref='stylesheet'">
<!-- 防止因禁用js导致样式加载失败展现无样式页面 -->
<noscript>
  <link rel="stylesheet" href="xxx.css">  
</noscript>
```

[loadcss](https://github.com/filamentgroup/loadCSS)

关键CSS

折叠指的是内容在屏幕上不可见的分界点，它还会基于查看页面的设备发生变化。
<link>标签会阻塞页面渲染,从而延迟文档的绘制。关键CSS可以缓解这种行为。其工作原理是优先加载折叠之上的首屏内容。通过将关键的样式内联到页面文档中，而非关键的样式则以延迟的方式加载。从而避免渲染阻塞的影响。
