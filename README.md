# 学习笔记  

## 搭建个人博客参考文章 [链接](https://mp.weixin.qq.com/s/pYKH4Go1ywsoWysLf_uNJg)

#### 1.[node.js安装与环境配置](https://www.jianshu.com/p/03a76b2e7e00)
#### 2.node.js win10安装出现问题 [解决方案1](https://blog.csdn.net/M075097/article/details/74910372) [解决方案2](https://www.jb51.net/article/99843.htm)，npm更新到最新版本的语句：“npm install npm@latest -g”，清除npm缓存语句：“npm cache clean -f”
#### 3.sublime text3 [安装packagecontrol](https://packagecontrol.io/installation) [注册](https://gist.github.com/cantgis/fb17ab10287c512379fbefad7fa5be1c) [汉化](https://www.jianshu.com/p/22e4db0f7b7b) windwos系统hosts文件路径为：C:\Windows\System32\drivers\etc 修改hosts文件：可将hosts文件先复制出来修改后再覆盖原来的即可
#### 4.sublime text3 前端插件 [力荐1](https://www.cnblogs.com/hykun/p/sublimeText3.html) [Emmet用法记忆表](https://docs.emmet.io/cheat-sheet/)
#### 5. 微信小程序豆瓣api请求问题，[参考这篇文章](https://blog.csdn.net/alisa7/article/details/80492410)
#### 6.gulp-sass编译时会间歇性的报错：找不到文件，[解决方案](https://www.cnblogs.com/venoral/p/6130353.html)
#### 7.webstrom IDE安装破解——使用破解补丁[参考网址1](https://blog.csdn.net/voke_/article/details/76418116)[参考网址2](https://www.jianshu.com/p/0bf76557153a)
#### 8.windows hosts文件路径：C:\Windows\System32\drivers\etc  修改hosts文件方法，复制出来修改，再覆盖回去
#### 9.iScroll插件使用 [中文文档](http://wiki.jikexueyuan.com/project/iscroll-5/gettingstart.html)
#### 10.better-scroll [中文文档](https://github.com/ustbhuangyi/better-scroll/blob/master/README_zh-CN.md)
#### 11.setTimeout(fn[,delay,param1,param2])，这个方法接收3个参数，前面两个比较熟悉，第三个参数是：一旦定时器到期，它们会作为参数传递给fn执行。
#### 12.gulp-sass 编译报错  [参考文章1](https://my.oschina.net/u/3149400/blog/1518298) [参考文章2](https://segmentfault.com/q/1010000008284566/a-1020000008285932) [参考文章3](https://zhuanlan.zhihu.com/p/25073197)
    Error: File to import not found or unreadable: module/header. on line 3 of src/style/style.scss
    >> @import "module/header";
       ^
#### 13.巧用margin/padding的百分比值实现高度自适应（多用于占位，避免闪烁）[链接](https://segmentfault.com/a/1190000004231995)
#### 14.可以写入到<head>标签的内容清单[参考链接](http://www.css88.com/archives/8052)[github](https://github.com/joshbuchea/HEAD)
#### 15.背景图固定，内容滚动且图片完整覆盖全屏--模仿百度首页。  
    HTML
    <body>
        <div class="skin"></div>
        <div class="container"></div>
    </body>
    
    css
    body {height: 100%}
    
    .skin {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: rgb(64, 64, 64);
        background-image: url(../../assets/images/login/login_bg.png);
        background-size: cover;
        background-position: center center;
        background-repeat: no-repeat;
        z-index: -10;
        zoom: 1;
    }
    
    .container {
        width: 100%;
        height: 1000px;
    }
    
#### 16.ul-li水平居中问题，设置li为float:left;display:inline;ul设置text-align:center;即可达到效果。
#### 17.响应式写轮播图列表，在一个外层box里写多个li，可以使用倍数选择器写不同的样式
#### 18.vue移动端打包路径的更改[参考网站](https://blog.csdn.net/qq_21785985/article/details/80579034)
#### 19.IScroll插件使用填坑如下：
* 先上一段官方文档的代码块
```html
    <div id="wrapper">
        <ul>
            <li>...</li>
            <li>...</li>
            ...
        </ul>
    </div>
```
```javascript
    <script type="text/javascript">
        var myScroll = new IScroll('#wrapper');
    </script>
```
* 说一下坑位：  
1.ul标签需要添加绝对定位和横向或纵向滚动的宽或高的样式，如果可以由li标签的宽或高撑开，也是可以的，或则通过js动态添加宽或高，不然就设置ul的宽或高大于#wrapper，只有ul某个方向的值大于#wrapper才能触发相应方向上的滚动事件。  
2.#wrapper最好设置相对定位的样式，承接上一步嘛，为ul绝对定位奠定基础  
3.最好延迟100ms后，再实例化，这样数据就加载完了，比较保险的做法
* 具体的[demo](https://github.com/cubiq/iscroll/tree/master/demos)
* 参考网址[网址1](http://caibaojian.com/iscroll-5/gettingstart.html) [网址2](https://blog.csdn.net/qq_36800701/article/details/79536983) [网址3](http://blog.51cto.com/cooca/1670508) [网址4](https://www.cnblogs.com/JoannaQ/p/3155873.html) [网址5](https://segmentfault.com/a/1190000003113280#articleHeader1)
#### 20.vscode编辑器加载文件夹时忽略node_modules文件夹，在这里[配置方法](https://stackoverflow.com/questions/30140112/how-do-i-hide-certain-files-from-the-sidebar-in-visual-studio-code/30142299#30142299)
#### 21.css3 appearance这个属性解决移动端自定义的select标签的样式，可以这样设置：appearance：none；[官方文档](http://www.w3school.com.cn/cssref/pr_appearance.asp)
#### 22.ios input设置成readonly后会有软盘的上下箭头出现在底部，需要在input内设置 unselectable="on" onfocus="this.blur()"
#### 23.瀑布流的布局使用css3属性
```
html
<ul class="content">
    <li></li>
    <li></li>
    <li></li>
</ul>

css
.content {
    column-count: 3;
    column-gap:0;
    li {
        break-inside: aviod;
    }
}
```
#### 24.iview 分页组件的使用的[参考网址](https://blog.csdn.net/u014418725/article/details/79702001)
#### 25.z-index 这个的意思都能理解，但是在特殊的用途上就忘记怎么灵活应用它了，例如，“美莱梦想家”的侧边栏导航的二级导航实现，须要在二级导航相对定位的元素中添加z-index，使得它层级变高，这样二级导航才不会被右边的内容遮挡住（我总觉得我明明发现的了问题的所在，但只是停留在表面，没有深入探究问题，所以在一个简单的显示隐藏问题上栽了跟头，最后请教大佬指点，才知道是这么个回事，就是在这个元素的父级设置了隐藏才显示不出来，^_^）
#### 26.cmder的安装教程 [参考网址](https://www.jianshu.com/p/5b7c985240a7)
#### 27.面试算法题，百度搜索《剑指offer》或者[leetcode](https://leetcode-cn.com/)
