# Flex
### flex 属性
> ## flex 容器属性
> * flex-direction 元素排列方向
>> 1. row 纵向 (默认值)
>> 2. column 横向
> * flex-wrap 元素换行（排列不下时）
>> 1. nowrap （默认值）
>> 1. wrap
>> 1. wrap-reverse
> * flex-flow flex-wrap和flex-direction的简写
> * just-content 元素在主(x)轴上的对齐方式
>> 1. flex-start 左对齐
>> 1. flex-end 右对齐
>> 1. center 居中
>> 1. space-around 元素间隔相等（两端也保持距离）
>> 1. space-between 元素间隔想等 （两端无距离）
>> 1. space-between 元素间隔想等 （两端无距离）
> * align-items 元素在交叉轴(y)上的对齐方式
>> 1. flex-start 左对齐
>> 1. flex-end 右对齐
>> 1. center 居中
>> 1. stretch 占满容器高度 （子元素不设置高度时）
>> 1. baseline 以文字的第一行基线对齐


> ## flex 元素属性
> * flex-grow 当有多余空间时，元素的放大比例
>> 整数0(默认值)、1、2、3...
> * flex-shrink 当空间不足时，元素的缩小比例
>> 整数1(默认值)、2、3...
> * flex-basis 元素在主轴上占据的空间
> * flex grow、shrink、basis的简写
> * order 元素排列顺序
> * align-self 元素自身对齐方式 (交叉轴)