# Transform
## 2d基本分类
* ###  旋转 (rotate)
    * transform: rotate(45deg); `顺时针`旋转45度
* ###  缩放 (scale)
    * transform: scale(0.5): `x和y轴`同时缩小一半
    * transform: scale(0.5T2): `x轴`缩小一半,`y轴`放大两倍
* ###  倾斜 (skew)
    * transform: skew(30deg); `x轴`向左倾斜30度，`y轴`不变
    * transform: skew(30deg,60deg); `x轴`向左倾斜30度，`y轴`向下倾斜60度
* ###  移动 (translate)
    * transform: translate(x,y); `x轴`移动x，`y轴`移动y
## 对同一元素使用多种形变
* 顺序不同，结果不同 (中心点和轴(旋转时坐标轴一起旋转)导致)
* transform: translate(300px,400px) rotate(45deg) scale(1.5);
* transform: rotate(45deg) translate(300px,400px) scale(1.5);

## transform-origin
*  修改变形的基准点，采用‘基准点在元素水平方向上的位置(left、center、right)，基准点在元素垂直方向上的位置’（top、center、bottom）
*  transform-origin:20% 40%;
*  transform-origin:left top;
## 3d基本分类
* ### 旋转（rotate）
    * rotateX
    * rotateY
    * rotateZ
* ### 缩放（scale）
    * scaleX
    * scaleY
    * scaleZ
* ### 倾斜（skew）
    * skewX
    * skewY
    * 元素不能在z轴上倾斜
* ### 移动（translate）
    * translateX
    * translateY
    * translateZ
## 变形矩阵 `matrix`
 * ### 计算2D变形
    * $\left|
      \begin{array}{lcr}
      a & b & c \\
      d & e & f
      \end{array}
      \right|$





