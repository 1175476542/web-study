# CSS
## 内联样式
1. 标签内使用style属性
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>内联样式</title>
</head>
<body>
    <p style = 'color: chartreuse;font-size: 50px'>一行字</p>
</body>
</html>
```
- 缺点：代码不便于复用，不推荐使用
2. 可以写到style标签里面
```html
    <style>
        .p{
            color: red;
            font-size: 20px;
        }
    </style>
```
## 外联样式
3. 可以写到外部的css文件中，并通过link标签引用
```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <link rel="stylesheet" href="./outer.css">
    <title>Document</title>
</head>
<body>
    <p>外联的样式</p>
</body>
</html>
```
## 选择器
### 通配符（优先级最小）0
### 标签选择器        1
### 类选择器         10
### id选择器        100 
```css
/*上述选择器示例*/
*{
    
}
body,header {
    margin: 0;
    padding: 0;
    text-align: center;
}

h1 {
    font-size: 30px;
    font-weight: bold;
}

.poet {
    font-size: 20px;
    color: gray;
}

#amazing1 {
    color: red;
}

```
### 交集选择器
```css
/*div下面的box类*/
div.box{
    
}
```
### 父子兄弟选择器