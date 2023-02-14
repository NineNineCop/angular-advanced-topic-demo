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
## 2022/08/12
### SPA
SPA： 单页面应用; 就是在一个项目中只有一个html页面, 它在第一次加载页面时, 将唯一完成的html页面和所有其余页面组件一起下载下来, 所有的组件的展示与切换都在这唯一的页面中完成, 这样切换页面时, 不会重新加载整个页面, 而是通过路由来实现不同组件之间的切换;  
angular
`<router-outlet></router-outlet>`就是SPA的体现;  
核心:  
更新视图而不重新请求页面;  
优点:  
用户体验好、快，内容的改变不需要重新加载整个页面;  
缺点:  
不利于搜索引擎的抓取;  
* 首次渲染速度相对较慢;  
hash 路由兼容梗好, 但是带#显得丑些, histroy 和正常 url 路径一样, 但是需要在服务器进行单独配置*(处理页面重载404问题);
#### https://juejin.cn/post/6844904151206330375

## 2022/10/27
HTML aside 内容应该与附近的内容相关


## 2023/02
en --- 使...
cor=com=con --- 来/共同
ab --- 离开/去
dis --- 反
ad --- 强调
pre --- 先前
pro --- 向前
ex=es --- 向外/出去
un=il --- 否定
cess=ces=ceed=ced --- 走
de --- 下/向下
merc --- 商业
man --- 人手
re --- 再/重新
