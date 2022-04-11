# html fundamental

### HTML 区块元素&内联元素：

<details>
<summary>区块元素</summary>

```
<address>        定义地址
<caption>        定义表格标题
<dd>        定义列表中定义条目
<div>        定义文档中的分区或节
<dl>        定义列表
<dt>        定义列表中的项目
<fieldset>        定义一个框架集
<form>        创建表单元素
<h1><h2><h3><h4><h5><h6>        标题元素
<hr>        水平线
<legend>        给fieldset元素定义标题
<li>        定义列表项目
<noframes>        为那些不支持框架的浏览器显示文本，放置于frameset标签内
<noscript>        为那些不支持脚本的浏览器显示文本
<ol>        有序列表
<ul>        无序列表
<p>        定义段落
<pre>        定义预格式化文本
<table>        定义表格
<tbody>        定义表格主体
<td>        表格中的标准单元格
<tr>        表格中的行
<tfoot>        表格中的页脚
<th>        定义表头单元格
<thead>        定义表格的表头
```
</details>
<details>
<summary>内联元素</summary>

```
<a>        可定义锚以及超链接
<abbr>        表示一个缩写形式
<acronym>        表示只取title中首字母的缩写形式
<b>        字体加粗
<bdo>        可覆盖默认的文本方向
<big>        大号字体加粗
<br>        换行
<cite>        引用进行定义
<code>        定义计算机代码文本
<dfn>        定义一个定义项目
<em>        定义为强调的内容
<i>        斜体文本效果
<img>        向网页中嵌入一张图像
<input>        输入框
<kbd>        定义键盘文本
<label>        为input进行标记/标注
<q>        定义短的引用

<s>    表示不准确不相关，却不应当给予删除的内容

<samp>        定义样本文本

<select>        定义单选或者多选菜单
<small>        呈现小号字体效果
<span>        组合文档中的行内元素
<strong>        语气更强的强调内容
<sub>        定义下标文本
<sup>        定义上标文本
<textarea>        多行文本输入控件
<tt>        打字机或者等宽的文本效果
<var>        定义变量
```
</details>

---

### css权重

每一个css的选择器都有一个相对的重要程度值，也就是权重的值，简称“权值”；

css通过css选择器的权重占比，来计算css选择规则的总权值，从而确定 定义样式规则的 优先级次序；

权重等级:

- 第一等级：代表 内联样式，如 style=""，权值为 1,0,0,0；

- 第二等级：代表 ID选择器，如 #id="", 权值为 0,1,0,0；

- 第三等级：代表 calss | 伪类 | 属性 选择器，如 .class | :hover,:link,:target | [type], 权值 0,0,1,0；

- 第四等级：代表 标签 | 伪元素 选择器，如 p | ::after, ::before, ::fist-inline, ::selection, 权值 0,0,0,1；

- 此外，通用选择器（*），子选择器（>）， 相邻同胞选择器（+）等选择器不在4等级之内，所以它们的权值都为 0,0,0,0；

权值比较 规则：
- 是从高到低逐级将等级位上的权重值
- 低等级的选择器，个数再多也不会越等级超过高等级的选择器的优先级的

---

### html 元素

https://developer.mozilla.org/en-US/docs/Web/HTML/Element

#### <mark>内容分区</mark>

`<article>`:The `<article>` HTML element represents a self-contained composition in a document, page, application, or site, which is intended to be independently distributable or reusable (e.g., in syndication). 

#### <mark>文本内容</mark>

`<blockquote>`.`cite`: This attribute is intended to point to information explaining the context or the reference for the quote.

`<dl>`: description list
`<dt>`: description term
`<dd>`: description detail

`<hr>`: represents a thematic break between <u>paragraph-level</u> elements

`<menu>`: is a semantic alternative to `<ul>`

`<pre>`: represents preformatted text which is to be presented exactly as written in the HTML file

#### <mark>内联文本<mark>

`<abbr>`: represents an abbreviation or acronym; the optional `title` attribute can provide an expansion or description for the abbreviation.

`<bdi>`: 双向隔离元素 ( `<bdi>` ) 告诉浏览器的<u>双向算法</u>将其包含的文本与周围的文本隔离，

`<bdo>`: 双向文本替代元素 (`<bdo>`) 改写了文本的方向性

`<cite>`: 引用（ Citation）标签 (`<cite>`) 表示一个作品的引用，且必须包含作品的标题。

`<data>`: 将一个指定内容和机器可读的翻译联系在一起

`<dfn>`: 定义元素 (`<dfn>`) 表示术语的一个定义。(一般与`<dt><dfn title="cascade"></dt>`连用)

`<kbd>`: 键盘输入元素 (`<kbd>`) 用于表示用户输入 (<kbd>ctrl</kbd>)

`<mark>`: 标记文本元素 (`<mark>`) 表示为引用或符号目的而标记或突出显示的文本，

`<ruby>`: 被用来展示东亚文字注音或字符注释。
`
<ruby>
  汉 <rp>(</rp><rt>han</rt><rp>)</rp>
  字 <rp>(</rp><rt>zi</rt><rp>)</rp>
</ruby>
`

`<s>`: (Strikethrough)使用删除线来渲染文本。

`<samp>`: 用于标识计算机程序输出

`<sub>`: (Subscript element) 与主要的文本相比，应该展示得更低并且更小。H<sub>2</sub>O

`<sup>`: (Superscript element) 与主要的文本相比，应该展示得更高并且更小。5<sup>2</sup>

`<u>`: (表意不清标注元素）表示一个需要标注为<u>非文本化（non-textual）</u>的内联文本域

`<var>`: 标签表示变量的名称

`<wbr>`: (Line Break Opportunity element) 其中浏览器可以选择来换行

#### <mark>图片和多媒体</mark>

`<map>`: 与 `<area>` 属性一起使用来定义一个图像映射 (一个可点击的链接区域).

`<area>`: 在图片上定义一个热点区域，可以关联一个超链接。

`<audio>`: 可以包含一个或多个音频资源,也可以使用 MediaStream 将这个元素用于流式媒体

- autoplay: 音频会尽快自动播放，不会等待整个音频文件下载完成。
- crossorigin: 支持cors
- anonymous: 在发送跨域请求时不携带验证信息
- use-credentials: 在发送跨域请求时携带验证信息
- currentTime: 属性将返回一个双精度浮点值，用以标明以秒为单位的当前音频的播放位置
- preload: `none` 不会缓存；`metadata` 获取长度；`auto` 缓存（默认）

`<track>`: 被当作媒体元素—audio 和 video的子元素来使用。它允许指定时序文本字幕

#### <mark>内嵌内容</mark>

`<iframe>`: 内联框架元素 (`<iframe>`) 表示嵌套的 (为了静态文本或svg)

`<embed>`: 外部内容嵌入元素 (可以被编程)

`<object>`: 嵌入对象元素 (for older browser)
 
`<picture>`: 通过包含零或多个 source 元素和一个 img 元素来为不同的显示/设备场景提供图像版本。浏览器会选择最匹配的子 `<source>` 元素，如果没有匹配的，就选择 `<img>` 元素的 src 属性中的 URL。

#### <mark>编辑标识</mark>

`<ins>`: 定义已经被插入文档中的文本。

#### <mark>表格</mark>

`<table>`: 属性

- align: `left`,`center`,`right`
- bgcolor
- border: 是否有边框
- cellpadding: 单元格padding
- cellspacing： 单元格间距 (边距坍缩)
- frame: 控制边框方向显示 (`above`,`lhs`,`box`...)
- rules: 定义了在一个表格中规则的显示位置 (`groups`,`rows`,`all`...)
- summary: 定义了一个替代文本

`<colgroup>`: 表格列组, 用来定义表中的一组列表 (可以给表格列加样式)


---

