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

## 结构性伪类选择器
* root
* not
* empty
* target
* first-child
* last-child
* nth-child
* nth-last-child
* nth-of-child
* nth-last-of-child
* only-child
### 伪类选择器
* link
* visited
* hover
* active
### 伪元素选择器
 > 选择器.类名：伪元素{属性：值}
* first-line
    * 向某个元素的第一行文字使用样式
* first-letter
    * 向某个元素的第一个文字使用样式
* before
    * 在某个元素之前插入一段内容
* after
    * 在某个元素之后插入一段内容
### 结构性伪类选择器
* root


