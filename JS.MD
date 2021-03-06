# JS初识

## JS定义
 
 javaScript是一门浏览器脚本语言，运行在浏览器上，是一门轻量级的弱类型(声明变量无需声明变量类型)语言，由三部分构成：ECMAScript(核心)，文档对象模型(DOM)，浏览器对象模型(BOM)。
 
## 浏览器工作原理

 浏览器运行→用户界面(点击操作)→渲染引擎(解析HTML和CSS)→JS解析器
 。
 
## JS的历史

 JS最初由网景公司创立，最初是为了实现一些验证。
 
## JS的`<script>`标签属性

- anync表示应立即下载脚本，但不应妨碍页面其他操作，如下载资源和等待加载其他脚本，只对外部脚本文件有效。

- defer表示脚本可以延迟到文档完全被解析和显示之后再执行，只对外部脚本文件有效，这个属性即使在IE7以前的更早版本也支持。

- src引入外部文件。

- type type=text/javascript。

## 使用`<script>`元素

> 一种是页面中嵌入javascript代码，另一种是引入外部javascript文件。

> 嵌入页面的javascript代码用`<script>`标签包裹，可以写在`<head>`标签里，也可以写在`<body>`标签里，一般用于页面初始化的代码写在上面，而用于页面效果的代码写在下面，等页面完全加载完毕以后在执行JS代码，避免出现js代码错误导致页面无法正常加载的情况。

## 注意

- 使用`<script>`嵌入javascript代码时，不要再代码任何地方出现`</script>`字符串，浏览器会认为是结束标签，如果需要使用，可以用转义符\解决这种问题。
