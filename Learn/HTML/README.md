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

