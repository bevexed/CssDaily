# 选择器
## 属性选择器
 使用属性选择器前，需要声明属性`att`和睡醒值`val`
 * \[att=val]
    * 如果元素用att表示的属性的属性值`等于`用val指定的字符，则该元素使用这个样式。
 * \[att*=val]
    * 如果元素用att表示的属性的属性值`包含`用val指定的字符，则该元素使用这个样式。
 * \[att^=val]
    * 如果元素用att表示的属性的属性值的`开头字符等于`用val指定的字符，则该元素使用这个样式。
 * \[att$=val]
    * 如果元素用att表示的属性的属性值的`结尾字符等于`用val指定的字符，则该元素使用这个样式。
    * 在指定匹配字符前必须加上`\`（例如：\[id = \\-1]）

## 伪元素选择器
 > 选择器.类名：伪元素{属性：值}
* first-line
    * 向某个元素的`第一行`文字使用样式
* first-letter
    * 向某个元素的`第一个`文字使用样式
* before
    * 在某个元素`之前`插入一段内容
* after
    * 在某个元素`之后`插入一段内容
## 伪类选择器
### 结构性伪类选择器
* root
    * 将样式绑定到页面的根元素中，在html中指包含整个页面的“\<html>”部分
        ```
        :root{background:black}
        ```
* not
    * 排除被选择的元素
        ```
        body * :not(h1){background:red} /*除了h1以外的元素，背景为红色*/
        ```
* empty
    * 当元素内容为空白时使用的样式
* target
    * 使用target选择器对页面中的某个target元素(该元素的id被当做页面中的超链接使用)指定样式，该样式只在用户点击了页面中超链接，并且跳转到页面中的target元素后生效。
    ```
    // css
    :target{background:red}
    // html
    <a href="text"></a>
    <div id='text'></div>
    ```
* first-child
* last-child
* nth-child(n)
* nth-last-child(n)

* nth-of-child(n)
* nth-last-of-child(n)
    * 只针对`同类型的子元素`进行选择
> n 可以为odd(基数)、even(偶数)、表达式(an+b)
* only-child
    * 当某个元素只有一个子元素时使用此样式

### UI元素状态伪类选择器
* a
    * link
    * visited
    * hover
    * active
* E:hover、E:active、E:focus
    * hover  当鼠标指针移动到元素上时元素所使用的样式
    * active 当鼠标指针在元素上摁下还没有松开时元素所使用的样式
    * focus  当元素获得光标时所使用的样式
* E:enabled、E:disabled
    * enabled  元素处于可用状态的样式
    * disabled 元素处于不可用状态的样式
* E:read-only、E:read-write
    * read-only  元素处于只读时的样式
    * read-write 元素处于非只读时的样式
* E:checked、E:default、E:indeterminate
    * checked radio或checkbox处于被选取时的状态
    * default 打开时默认处于选取状态的样式
    * indeterminate 当页面打开时，一组单选框中没有任何一个单选框被设定为选取状态时整组单选框的样式。
* E::selection
    * 指定元素被选中时的样式[案例](../selection.html)
