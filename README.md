# Normalize.css
## 1. 什么是Normalize.css？
>定义浏览器统一的默认样式：Normalize.css
1. 如果你从事网页前端工作，肯定会发现不同浏览器的默认样式有细微的差异，这个让你在使用 CSS 进行布局工作的时候相当烦人，况且有些差异还不是那么细微，比如不同浏览器之间的默认表单样式差异以及 <html> 和 <body> 元素的margin 和 padding 的差异等。  
2. 一般前端工程师都会使用 reset.css 去处理不同浏览器的默认样式，这里推荐使用 Normalize.css，它是一个定制的 reset.css 文件，可以让所有元素在所有的现代浏览器上渲染一致。
3. 相比其它的 reset.css，Normalize.css 保留有用的默认样式，不像其它 reset.css 那么彻底，移除了每个默认样式，然后又得费神把需要的样式再加回来。Normalize.css 定义绝大多数元素的默认样式，并且还提高了一些元素的可用性，并且代码都有详细的注释。

## 2. Normalize.css 支持的浏览器
* Google Chrome (latest)
* Mozilla Firefox (latest)
* Mozilla Firefox 4
* Opera (latest)
* Apple Safari 6+
* Internet Explorer 8+
## 3. 如何使用 Normalize.css
Normalize.css 使用非常非常简单.    
首先，安装或从Github下载Normalize.css，接下来有两种主要途径去使用它。

策略一：将normalize.css作为你自己项目的基础CSS，自定义样式值以满足设计师的需求。  
策略二：引入normalize.css源码并在此基础上构建，在必要的时候用你自己写的CSS覆盖默认值。  
`<link rel="stylesheet" href="https://necolas.github.io/normalize.css/8.0.0/normalize.css"`
***
/ *！normalize.css v8.0.0 | MIT许可证| github.com/necolas/normalize.css * /

/ *文件
   ================================================== ======================== * /

/ **
 * 1.更正所有浏览器中的行高。
 * 2.在iOS中改变方向后，不要调整字体大小。
 * /

html {
  行高：1.15; / * 1 * /
  -webkit-text-size-adjust：100％; / * 2 * /
}

/ *部分
   ================================================== ======================== * /

/ **
 *删除所有浏览器的保证金。
 * /

身体 {
  保证金：0;
}

/ **
 *修改`section`内的`h1`元素的字体大小和边距
 * Chrome，Firefox和Safari中的`article`上下文。
 * /

h1 {
  font-size：2em;
  保证金：0.67em 0;
}

/ *分组内容
   ================================================== ======================== * /

/ **
 * 1.在Firefox中添加正确的框尺寸。
 * 2.在Edge和IE中显示溢出。
 * /

hr {
  方块大小：内容框; / * 1 * /
  身高：0; / * 1 * /
  溢出：可见; / * 2 * /
}

/ **
 * 1.纠正所有浏览器中字体大小的继承和缩放。
 * 2.更正所有浏览器中奇怪的'em`字体大小。
 * /

pre {
  font-family：等宽字体，等宽字体; / * 1 * /
  font-size：1em; / * 2 * /
}

/ *文本级语义
   ================================================== ======================== * /

/ **
 *删除IE 10中活动链接上的灰色背景。
 * /

一个 {
  background-color：transparent;
}

/ **
 * 1.删除Chrome 57-
 * 2.在Chrome，Edge，IE，Opera和Safari中添加正确的文字修饰。
 * /

abbr [title] {
  border-bottom：none; / * 1 * /
  文字修饰：下划线; / * 2 * /
  文字装饰：点缀下划线; / * 2 * /
}

/ **
 *在Chrome，Edge和Safari中添加正确的字体重量。
 * /

b，
强{
  font-weight：bold;
}

/ **
 * 1.纠正所有浏览器中字体大小的继承和缩放。
 * 2.更正所有浏览器中奇怪的'em`字体大小。
 * /

码，
大骨节病，
samp {
  font-family：等宽字体，等宽字体; / * 1 * /
  font-size：1em; / * 2 * /
}

/ **
 *在所有浏览器中添加正确的字体大小。
 * /

小{
  字体大小：80％;
}

/ **
 *防止`sub`和`sup`元素影响行中的高度
 *所有浏览器。
 * /

子，
sup {
  font-size：75％;
  line-height：0;
  位置：相对;
  vertical-align：baseline;
}

sub {
  底部：-0.25em;
}

sup {
  顶部：-0.5em;
}

/ *嵌入式内容
   ================================================== ======================== * /

/ **
 *删除IE 10中链接内的图像边框。
 * /

img {
  border-style：none;
}

/* 形式
   ================================================== ======================== * /

/ **
 * 1.更改所有浏览器中的字体样式。
 * 2.删除Firefox和Safari中的边距。
 * /

按钮，
输入，
OPTGROUP，
选择，
textarea {
  font-family：inherit; / * 1 * /
  font-size：100％; / * 1 * /
  行高：1.15; / * 1 * /
  保证金：0; / * 2 * /
}

/ **
 *在IE中显示溢出。
 * 1.在Edge中显示溢出。
 * /

按钮，
输入{/ * 1 * /
  溢出：可见;
}

/ **
 *删除Edge，Firefox和IE中文本转换的继承。
 * 1.删除Firefox中文本转换的继承。
 * /

按钮，
选择{/ * 1 * /
  text-transform：none;
}

/ **
 *更正无法在iOS和Safari中设置可点击类型的风格。
 * /

按钮，
[类型= “按钮”]，
[类型= “复位”]，
[type =“submit”] {
  -webkit-appearance：button;
}

/ **
 *在Firefox中删除内部边框和填充。
 * /

按钮::  -  MOZ-焦点内，
[类型= “按钮”] ::  -  MOZ-焦点内，
[类型= “复位”] ::  -  MOZ-焦点内，
[type =“submit”] ::  -  moz-focus-inner {
  border-style：none;
  填充：0;
}

/ **
 *恢复先前规则未设置的焦点样式。
 * /

按钮：-moz-focusring，
[类型= “按钮”]： -  MOZ-focusring，
[类型= “复位”]： -  MOZ-focusring，
[type =“submit”]： -  moz-focusring {
  大纲：1px点缀ButtonText;
}

/ **
 *更正Firefox中的填充。
 * /

fieldset {
  填充：0.35em 0.75em 0.625em;
}

/ **
 * 1.更正Edge和IE中的文字换行。
 * 2.更正IE中`fieldset`元素的颜色继承。
 * 3.删除填充，以便在开发人员将它们清零时不会被捕获
 *所有浏览器中的`fieldset`元素。
 * /

传奇{
  盒子尺寸：边框; / * 1 * /
  颜色：继承; / * 2 * /
  显示：表格; / * 1 * /
  最大宽度：100％; / * 1 * /
  填充：0; / * 3 * /
  空白：正常; / * 1 * /
}

/ **
 *在Chrome，Firefox和Opera中添加正确的垂直对齐。
 * /

进展{
  vertical-align：baseline;
}

/ **
 *删除IE 10+中的默认垂直滚动条。
 * /

textarea {
  溢出：自动;
}

/ **
 * 1.在IE 10中添加正确的框大小。
 * 2.删除IE 10中的填充。
 * /

[类型= “复选框”]，
[type =“radio”] {
  盒子尺寸：边框; / * 1 * /
  填充：0; / * 2 * /
}

/ **
 *修正Chrome中增加和减少按钮的光标风格。
 * /

[TYPE = “号码”] ::  -  WebKit的内自旋按钮，
[type =“number”] ::  -  webkit-outer-spin-button {
  身高：自动;
}

/ **
 * 1.更正Chrome和Safari中奇怪的外观。
 * 2.更正Safari中的大纲样式。
 * /

[type =“search”] {
  -webkit-appearance：textfield; / * 1 * /
  outline-offset：-2px; / * 2 * /
}

/ **
 *在macOS上删除Chrome和Safari中的内部填充。
 * /

[type =“search”] ::  -  webkit-search-decoration {
  -webkit-appearance：none;
}

/ **
 * 1.纠正无法在iOS和Safari中设置可点击类型的风格。
 * 2.在Safari中将字体属性更改为`inherit`。
 * /

::  -  webkit-file-upload-button {
  -webkit-appearance：button; / * 1 * /
  font：inherit; / * 2 * /
}

/ *互动
   ================================================== ======================== * /

/ *
 *在Edge，IE 10+和Firefox中添加正确的显示。
 * /

细节 {
  显示：块;
}

/ *
 *在所有浏览器中添加正确的显示。
 * /

汇总{
  display：list-item;
}

/ *杂项
   ================================================== ======================== * /

/ **
 *在IE 10+中添加正确的显示。
 * /

模板{
  显示：无;
}

/ **
 *在IE 10中添加正确的显示。
 * /

[hidden] {
  显示：无;
}
