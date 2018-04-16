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
/*! normalize.css v8.0.0 | MIT License | github.com/necolas/normalize.css */
## 说明：normalize文档可拆分为不同的模块来使用.
1. [Document](#Document)
2. [Sections](#Sections)  
3. [Grouping content](#Groupingcontent)
4. [Text-level semantics](#Text-levelsemantics)
5. [Embedded content](#Embeddedcontent)
6. [Forms](#Forms)
7. [Interactive](#Interactive)
8. [Misc](#Misc)  
  
/* ========================================================================== */

### /* <a id="Document">1. Document</a> */

/*
 * 1. Correct the line height in all browsers.
 * .修正所有浏览器中的行高。
 * 2. Prevent adjustments of font size after orientation changes in iOS.
 * .在iOS中改变方向后，不要调整字体大小。
 */

html {
  line-height: 1.15; /* 1 */
  -webkit-text-size-adjust: 100%; /* 2 */
}

/* ========================================================================== */

### /* <a id="Sections">2. Sections</a>*/

/*
 * Remove the margin in all browsers.
 */

body {
  margin: 0;
}

/*
 * Correct the font size and margin on `h1` elements within `section` and
 * `article` contexts in Chrome, Firefox, and Safari.
 * 修正Chrome，Firefox和Safari中的`section`和*`article`上下文中`h1`元素的字体大小和边距。
 */

h1 {
  font-size: 2em;
  margin: 0.67em 0;
}

/* ========================================================================== */

### /* <a id="Groupingcontent">3. Grouping content</a>*/

/*
 * 1. Add the correct box sizing in Firefox.
 * 2. Show the overflow in Edge and IE.
 */

hr {
  box-sizing: content-box; /* 1 */
  height: 0; /* 1 */
  overflow: visible; /* 2 */
}

/*
 * 1. Correct the inheritance and scaling of font size in all browsers.
 * 2. Correct the odd `em` font sizing in all browsers.
 * .纠正所有浏览器中字体大小的继承和缩放。
 * .更正所有浏览器中奇怪的'em`字体大小。
 * pre标签适合显示计算机代码
 */

pre {
  font-family: monospace, monospace; /* 1 */
  font-size: 1em; /* 2 */
}

/* ========================================================================== */

### /* <a id="Text-levelsemantics">4. Text-level semantics</a> */

/*
 * Remove the gray background on active links in IE 10.
 * 删除IE 10中活动链接上的灰色背景。
 */

a {
  background-color: transparent;
}

/*
 * 1. Remove the bottom border in Chrome 57-
 * 2. Add the correct text decoration in Chrome, Edge, IE, Opera, and Safari.
 * <abbr> 标签指示简称或缩写，比如 "baidu"。
 * <abbr title="https://baidu.com">baidu</abbr>
 */

abbr[title] {
  border-bottom: none; /* 1 */
  text-decoration: underline; /* 2 */
  text-decoration: underline dotted; /* 2 */
}

/*
 * Add the correct font weight in Chrome, Edge, and Safari.
 * 在Chrome，Edge和Safari中添加正确的字体重量。
 */

b,
strong {
  font-weight: bolder;
}

/*
 * 1. Correct the inheritance and scaling of font size in all browsers.
 * 2. Correct the odd `em` font sizing in all browsers.
 * monospace 等宽字体
 */

code,
kbd,
samp {
  font-family: monospace, monospace; /* 1 */
  font-size: 1em; /* 2 */
}

/*
 * Add the correct font size in all browsers.
 */

small {
  font-size: 80%;
}

/*
 * Prevent `sub` and `sup` elements from affecting the line height in
 * all browsers.
 * 在所有的浏览器中，防止`sub`和`sup`元素影响行中的高度
 */

sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}

sub {
  bottom: -0.25em;
}

sup {
  top: -0.5em;
}

/* ========================================================================== */

### /* <a id="Embeddedcontent">5. Embedded content</a> */

/*
 * Remove the border on images inside links in IE 10.
 *  *删除IE 10中链接内的图像边框。
 */

img {
  border-style: none;
}

/* ========================================================================== */

### /* <a id="Forms">6. Forms</a> */

/*
 * 1. Change the font styles in all browsers.
 * 2. Remove the margin in Firefox and Safari.
 */

button,
input,
optgroup,
select,
textarea {
  font-family: inherit; /* 1 */
  font-size: 100%; /* 1 */
  line-height: 1.15; /* 1 */
  margin: 0; /* 2 */
}

/*
 * Show the overflow in IE.
 * 1. Show the overflow in Edge.
 */

button,
input { /* 1 */
  overflow: visible;
}

/*
 * Remove the inheritance of text transform in Edge, Firefox, and IE.
 * 1. Remove the inheritance of text transform in Firefox.
 */

button,
select { /* 1 */
  text-transform: none;
}

/*
 * Correct the inability to style clickable types in iOS and Safari.
 */

button,
[type="button"],
[type="reset"],
[type="submit"] {
  -webkit-appearance: button;
}

/*
 * Remove the inner border and padding in Firefox.
 */

button::-moz-focus-inner,
[type="button"]::-moz-focus-inner,
[type="reset"]::-moz-focus-inner,
[type="submit"]::-moz-focus-inner {
  border-style: none;
  padding: 0;
}

/*
 * Restore the focus styles unset by the previous rule.
 */

button:-moz-focusring,
[type="button"]:-moz-focusring,
[type="reset"]:-moz-focusring,
[type="submit"]:-moz-focusring {
  outline: 1px dotted ButtonText;
}

/*
 * Correct the padding in Firefox.
 */

fieldset {
  padding: 0.35em 0.75em 0.625em;
}

/*
 * 1. Correct the text wrapping in Edge and IE.
 * 2. Correct the color inheritance from `fieldset` elements in IE.
 * 3. Remove the padding so developers are not caught out when they zero out
 *    `fieldset` elements in all browsers.
 */

legend {
  box-sizing: border-box; /* 1 */
  color: inherit; /* 2 */
  display: table; /* 1 */
  max-width: 100%; /* 1 */
  padding: 0; /* 3 */
  white-space: normal; /* 1 */
}

/*
 * Add the correct vertical alignment in Chrome, Firefox, and Opera.
 */

progress {
  vertical-align: baseline;
}

/*
 * Remove the default vertical scrollbar in IE 10+.
 */

textarea {
  overflow: auto;
}

/*
 * 1. Add the correct box sizing in IE 10.
 * 2. Remove the padding in IE 10.
 */

[type="checkbox"],
[type="radio"] {
  box-sizing: border-box; /* 1 */
  padding: 0; /* 2 */
}

/*
 * Correct the cursor style of increment and decrement buttons in Chrome.
 */

[type="number"]::-webkit-inner-spin-button,
[type="number"]::-webkit-outer-spin-button {
  height: auto;
}

/*
 * 1. Correct the odd appearance in Chrome and Safari.
 * 2. Correct the outline style in Safari.
 */

[type="search"] {
  -webkit-appearance: textfield; /* 1 */
  outline-offset: -2px; /* 2 */
}

/*
 * Remove the inner padding in Chrome and Safari on macOS.
 */

[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}

/*
 * 1. Correct the inability to style clickable types in iOS and Safari.
 * 2. Change font properties to `inherit` in Safari.
 */

::-webkit-file-upload-button {
  -webkit-appearance: button; /* 1 */
  font: inherit; /* 2 */
}

/* ========================================================================== */

### /* <a id="Interactive">7. Interactive</a> */

/*
 * Add the correct display in Edge, IE 10+, and Firefox.
 */

details {
  display: block;
}

/*
 * Add the correct display in all browsers.
 */

summary {
  display: list-item;
}

/* ========================================================================== */

### /* <a id="Misc">8. Misc</a> */

/*
 * Add the correct display in IE 10+.
 */

template {
  display: none;
}

/*
 * Add the correct display in IE 10.
 */

[hidden] {
  display: none;
}
