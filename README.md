# Normalize.css
## 1. 什么是Normalize.css？
>定义浏览器统一的默认样式：Normalize.css
1. 如果你从事网页前端工作，肯定会发现不同浏览器的默认样式有细微的差异，这个让你在使用 CSS 进行布局工作的时候相当烦人，况且有些差异还不是那么细微，比如不同浏览器之间的默认表单样式差异以及 <html> 和 <body> 元素的margin 和 padding 的差异等。  
2. 一般前端工程师都会使用 reset.css 去处理不同浏览器的默认样式，这里推荐使用 Normalize.css，它是一个定制的 reset.css 文件，可以让所有元素在所有的现代浏览器上渲染一致。
3. 相比其它的 reset.css，Normalize.css 保留有用的默认样式，不像其它 reset.css 那么彻底，移除了每个默认样式，然后又得费神把需要的样式再加回来。Normalize.css 定义绝大多数元素的默认样式，并且还提高了一些元素的可用性，并且代码都有详细的注释。

## 2.Normalize.css 支持的浏览器
* Google Chrome (latest)
* Mozilla Firefox (latest)
* Mozilla Firefox 4
* Opera (latest)
* Apple Safari 6+
* Internet Explorer 8+
## 如何使用 Normalize.css
Normalize.css 使用非常简单，并且七牛的 StaticFile.org 已经包含了该库，所以无需下载，只要在网页的头部加入以下代码即可：  

<link rel="stylesheet" href="http://cdn.staticfile.org/normalize/3.0.1/normalize.min.css" t
