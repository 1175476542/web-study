# HTML
1. mata
- 自结束标签
- charset：字符设置
- 设置网页中的元数据，他的内容不被用户查看，一般用来高速浏览器如何解析网页，或者告诉搜索引擎网页的主要内容
- 可选属性：
  - name：要设置的属性的名字
  - content：要设置属性的内容
  - description：用于告诉搜索引擎网页的主要内容
  - keywords：关键词，告诉浏览器搜索引擎的关键词
  - http-equiv：用来重定向
- 在html中多个空格和换行符会被解析为一个空格
## 标题标签
1. h1-h6
```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>标题标签</title>
</head>
<body>
    <h1>一级标题</h1>
    <h2>一级标题</h2>
    <h3>一级标题</h3>
    <h4>一级标题</h4>
    <h5>一级标题</h5>
    <h6>一级标题</h6>
</body>
</html>
```
2. 段落标签
- 独占一行
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Param</title>
</head>
<body>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
    <p>我是一个段落</p>
</body>
</html>
```
3. <br>:换行符
4. <hr>:本来表示水平线，h5表示分割线
5. 转义字符
- &nbsp：表示空格
- &gt：大于号
- &lt：小于号
- &copy：版权符号
# 语义化标签
1. header
2. footer
3. aside
4. nav
5. main
> 一般没有什么变化，多数就是一种规范
## 图片
### 语法格式
```html
<img src="./xx.jpg" alt="文字提醒">
```
> 文字题形式加载不出或者不兼容时显示
## audio
### 语法格式(两种)
```html
<audio controls src="./audio.mp3"></audio>
```
```html
<audio controls>
  提示信息
  <source  src="./audio.mp3">
  <source  src="./audio.ogg">
  <embed src="./audio.ogg" type="audio/mp3" width = "300" height="300">
</audio>
```
- 可以给很多格式，如果都不支持，显示提示信息
### 属性
1. controls
- 用来设置是否允许用户控制音频的播放，没有属性值
2. autoplay
- 自动播放
3. loop
- 循环
## video
### 语法格式(两种)
```html
<video controls src="./audio.mp4"></video>
```
```html
<video controls>
  提示信息
  <source  src="./audio.mp4">
  <source  src="./audio.webm">
  <embed src="./audio.mp4" type="audio/mp4" width = "300" height="300">
</video>
```
### 属性
1. controls
- 用来设置是否允许用户控制音频的播放，没有属性值
2. autoplay
- 自动播放
3. loop
- 循环
## 超链接
- 可以从一个页面跳转到另一个页面
### 语法格式
```html
<a href="www.baidu.com">跳转到百度</a>
```
### 属性
1. href= "指定路径"：指定跳转路径
- href = "#"：跳转当前页面顶部
- href = "#{id}":跳转到指定id，如bottom，或id=p1的标签
2. target：表示打开链接的位置
- _self:默认值，在当前页面打开
- _blank:在新窗口打开
## 列表