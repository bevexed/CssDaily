# Before & After
* before 和 after 在页面中的元素的前面和后面插入内容
* content 属性来定义插入的具体内容
### 插入文字
```
h1:before{
    content:'1'
}

/*指定个别元素不插入*/
h1:before{
    content:none
}
```
### 插入图片
```
h1:before{
    content:url(123.png)
}

/*用alt属性值作为图片的标题显示*/
img:after{
    content:attr(alt);
    display:block;
    text-align:center;
    margin-top:5px;
}
```
### 插入项目符号
* 在多个标题前加连续编号
```
<元素>:before{
    content: counter(计数器名字)
}

<元素>:{
    counter-increment:before或after选择器中计数器的名字
}
```
* 在项目编号中加文字
```
h1{
    counter-increment: aaa;
}
h1:before{
    content: '第'counter(aaa)'章'';
}
```
* 指定编号种类
    * counter(计数器名，编号种类)
    * upper-alpha(大写字母编号)
    * upper-roman(大写罗马字母编号)
* 编号嵌套
    * counter-reset

