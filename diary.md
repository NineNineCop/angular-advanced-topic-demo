## 2022/08/10
#### https://juejin.cn/post/7128369638794231839#heading-5
### 客户端渲染 CSR
动态渲染, 也就是平时我们所称的客户端渲染 CSR;
### 静态站点生成 SSG
静态渲染, HTML文档在项目build打包构建时就已经生成好了, 用户请求的时候服务端不需要再发送其它请求和进行二次组装, 直接将该HTML文档响应给客户端即可;
### preload
eg: <link as="script" rel="preload" href="js">
as 值是必须的;
### preconnect
eg: <link rel="preconnect" href="xxx">
提示浏览器用户可能需要来自目标域名的资源, 因此浏览器可以通过抢先启动与该域名的连接来改善用户体验 -- MDN;
### prefetch
eg: <link rel="prefetch" href="/.json" crossorigin="anonymous" as="fetch">
提示浏览器，用户未来的浏览有可能需要加载目标资源，所以浏览器会事先获取和缓存对应资源，优化用户体验 -- MDN;
### npm run
运行 npm run xxx 的时候, npm 会先在当前目录的 node_modules/.bin 查找要执行的程序, 如果找到则运行, 找不到则全局找目录的 node_modules/.bin;
本质还是启动脚本;
## 2022/08/11
### CSS改变默认文本选中的颜色
```
.xxx::selection {
    background:xxx;
    color:#fff;
}
```
