# HTML 学习笔记



# 1. HTML 基础

## 1.1 HTML: 

超文本标记语言，HyperText Marked Language。

## 1.2 `<!DOCTYPE>` 声明:

用来声明HTML的版本，该声明不区分大小写。如HTML5的声明为：

```html
<!DOCTYPE html>
```



## 1.3 中文编码

在头标签<head>中声明中文编码：

```html
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>页面标题</title>
</head>
<body>
 
<h1>我的第一个标题</h1>
 
<p>我的第一个段落。</p>
 
</body>
</html>
```



## 1.4 标题

HTML中的标题通过`<h1>-<h6>`标签来定义。

```html
<h1>一级标题</h1>
<h2>二级标题</h2>
```

## 1.5 段落

段落通过`<p>`标签来定义。

```html
<p>我的第一个段落。</p>
<p>我的第二个段落。</p>
```

## 1.6 链接

链接通过`<a>`标签来定义。

```html
<a href="https://yangshaoxiong.tech">这是一个链接</a>
```

## 1.7 图像

图像用`<img>`标签来定义。

```html
<img src="/images/logo.png" width="258" height="39" />
```

# 2. HTML 元素

HTML 文档由 HTML 元素定义。

`<html>` 元素定义了整个 HTML 文档。

没有内容的 HTML 元素被称为空元素。空元素是在开始标签中关闭的。

**推荐使用小写标签：**

HTML 标签对大小写不敏感，推荐使用小写标签。

# 3. HTML 属性

属性是 HTML 元素提供的附加信息。

- HTML 元素可以设置**属性**
- 属性可以在元素中添加**附加信息**
- 属性一般描述于**开始标签**
- 属性总是以名称/值对的形式出现，**比如：name="value"**。
- 属性值应该始终被包括在引号内。
- 双引号是最常用的，不过使用单引号也没有问题。(在某些个别的情况下，比如属性值本身就含有双引号，那么您必须使用单引号，例如：name='John "ShotGun" Nelson')
- 属性和属性值对大小写不敏感。推荐使用小写。

eg. HTML 链接由 `<a>`标签定义。链接的地址在 **href 属性**中指定：

```
<a href="http://www.runoob.com">这是一个链接</a>
```



# 4. HTML 标签

## 4.1 超链接 `<a>`

超链接可以是一个字，一个词，或者一组词，也可以是一幅图像，您可以点击这些内容来跳转到新的文档或者当前文档中的某个部分。

eg.

```html
<a href="https://yangshaoxiong.tech">我的博客地址</a>
```

超链接的属性：

| 属性     | 描述                                                         |
| -------- | ------------------------------------------------------------ |
| href     | 链接的目标 URL，可以是网页url，或者图片，HTML元素等          |
| target   | 规定在何处打开目标 URL。仅在 href 属性存在时使用。<br/>`_blank`：新窗口打开。<br/>`_parent`：在父窗口中打开链接。<br/>`_self`：默认，当前页面跳转。<br/>`_top`：在当前窗体打开链接，并替换当前的整个窗体(框架页)。 |
| download | 指定下载链接                                                 |
| type     | 规定目标 URL 的 MIME 类型。仅在 href 属性存在时使用。        |
| id       | 可用于创建一个 HTML 文档书签，使用#来实现同一个页面不同位置的跳转。 |

## 4.2 头部



| 标签       | 描述                                                         |
| ---------- | ------------------------------------------------------------ |
| `<head>`   | 表示HTML 头部                                                |
| `<title>`  | 标题                                                         |
| `<base>`   | 描述了基本的链接地址/链接目标，该标签作为HTML文档中所有的链接标签的默认链接 |
| `<link>`   | 定义了文档与外部资源之间的关系，通常用于链接到样式表         |
| `<style>`  | 定义了HTML文档的样式文件引用地址                             |
| `<meta>`   | 描述了一些基本的元数据                                       |
| `<script>` | 用于加载脚本文件，如： JavaScript                            |

- title元素，定义了浏览器工具栏的标题；当网页添加到收藏夹时，显示在收藏夹中的标题；显示在搜索引擎结果页面的标题。
- base元素，描述了基本的链接地址/链接目标，该标签作为HTML文档中所有的链接标签的默认链接:

## 4.3 CSS

CSS：层叠样式表（Cascading Style Sheets）

CSS 添加到HTML的方式：

- 内联样式：在HTML元素中使用"style"属性
- 内部样式表：在HTML文档头部`<head>`区域使用`<style>`元素来包含CSS
- 外部引用：使用外部CSS文件（推荐使用）

部分常用属性：

- color：颜色
- margin_left：左边距
- background-color：背景颜色
- font-family：字体
- font-size：字体大小
- text-align：文字对齐

## 4.4 图像

HTML中图像使用标签`<img>`表示。

`<img>` 是空标签，意思就是它只包含属性，没有闭合标签。

图像相关属性：

- src：表示图像的地址，可以为本地文件，也可以为网络上的文件。
- alt：用来为图像定义一串预备的可替换的文本。如当浏览器不能正常载入图像时，替换文本属性告诉读者她们失去的信息。此时，浏览器将显示这个替代性的文本而不是图像。
- height：高度。
- width：宽度。

eg.

```html
    <h2>Norwegian Mountain Trip</h2>
    <img border="0" src="./resources/images/pulpit.jpg" alt="Pulpit rock" width="304" height="228">

    <p>网络上的图片</p>
    <img src="https://avatars.githubusercontent.com/u/8236175?s=400&u=4ef8ad6e72966ea14cb197e986cff78fb4ca9e6e&v=4"
     alt="avatar youngbear" width="400" height="400">
```

图像链接：使用`<a>`和`<img>`组合：

```html
    <p>图像链接</p>
    <a href="https://github.com/YoungBear">
        <img src="./resources/images/avatar.jfif" height="30" width="30"></a>
```

## 4.5 表格

- 表格由标签`<table>`来定义
- 行由`<tr>`来定义
- 每行由标签`<td>`表示若干单元格（table data）
- 数据单元格可以包含文本，图片，列表，段落，表单，水平线，表格等
- 标签`<border>`表示边框
- 标签`<th>`表示表头
- `<caption>`表示表格标题

eg.

```html
    <p>2行3列的表格</p>
    <table border="1">
        <tr>
            <th>表头1</th>
            <th>表头2</th>
            <th>表头3</th>
        </tr>
        <tr>
            <td>aa</td>
            <td>ab</td>
            <td>ac</td>
        </tr>
        <tr>
            <td>ba</td>
            <td>bb</td>
            <td>bc</td>
        </tr>
    </table>
```

参考：[HTML表格](https://www.runoob.com/html/html-tables.html)

## 4.6 列表

HTML 支持有序、无序和定义列表:

无序列表是一个项目的列表，此列项目使用粗体圆点（典型的小黑圆圈）进行标记。无序列表使用 `<ul>` 标签。

同样，有序列表也是一列项目，列表项目使用数字进行标记。 有序列表始于 `<ol> `标签。每个列表项始于 `<li> `标签。

自定义列表不仅仅是一列项目，而是项目及其注释的组合。

自定义列表以 `<dl>` 标签开始。每个自定义列表项以 `<dt>` 开始。每个自定义列表项的定义以 `<dd>` 开始。

列表相关标签：

| 标签   | 描述                                        |
| ------ | ------------------------------------------- |
| `<ol>` | 定义有序列表 ordered lists                  |
| `<ul>` | 定义无序列表 unordered lists                |
| `<li>` | 定义列表项 list item                        |
| `<dl>` | 子定义列表 definition lists                 |
| `<dt>` | 自定义列表项目 definition term              |
| `<dd>` | 定义自定列表项的描述 definition description |



```html
<body>
    <h4>无序列表:</h4>
    <ul>
        <li>Coffee</li>
        <li>Tea</li>
        <li>Milk</li>
    </ul>

    <h4>有序列表:</h4>
    <ol>
        <li>Coffee</li>
        <li>Tea</li>
        <li>Milk</li>
    </ol>

    <h4>有序列表:指定起始序号</h4>
    <ol start="20">
        <li>Coffee</li>
        <li>Tea</li>
        <li>Milk</li>
    </ol>

    <h4>一个自定义列表：</h4>
    <dl>
        <dt>Coffee</dt>
        <dd>- black hot drink</dd>
        <dt>Milk</dt>
        <dd>- white cold drink</dd>
    </dl>
</body>
```



## 4.7 div

HTML元素：

- 块级元素：会以新行开始和结束。如h1,p。
- 内联元素：不会以新行开始。如img。

`div` 是块级元素，可用于组合其他HTML元素的容器。

`span` 元素是内联元素，可用作文本的容器。

```html
    <div style="color:#0000FF">
        <h3>这是一个在 div 元素中的标题。</h3>
        <p>这是一个在 div 元素中的文本。</p>
    </div>
    <p>我的母亲有 <span style="color:blue">蓝色</span> 的眼睛。</p>
```



