# 学习笔记  

## 搭建个人博客参考文章 [链接](https://mp.weixin.qq.com/s/pYKH4Go1ywsoWysLf_uNJg)

#### 1.[node.js安装与环境配置](https://www.jianshu.com/p/03a76b2e7e00)
#### 2.node.js win10安装出现问题 [解决方案1](https://blog.csdn.net/M075097/article/details/74910372) [解决方案2](https://www.jb51.net/article/99843.htm)
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
