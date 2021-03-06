# 1.认识flex
![](_v_images/20200610133925151_16583.png)

# 2.flex布局模型
主要理解主轴与交叉轴的概念
![](_v_images/20200610135228140_31010.png)
## 1.主轴：
主轴与交叉轴是互相垂直的关系。主轴的方向是不固定的，使用起始线和终止线来描述。
主轴的方向由`flex-direction`来定义,可取4个值定义:
- row
- row-reverse
- column
- column-reverse

如果选择了`row`或者`row-reverse`，那么主轴方向将沿着 `inline`方向延伸。
![](_v_images/20200610135905702_11402.png)

如果选择的是 `column` 或者 `column-reverse`时，主轴方向会沿着上下方向延伸，也就是 `block` 块排列的方向
![](_v_images/20200610140055926_31187.png)

## 2.交叉轴：
交叉轴垂直于主轴。
如果flex-direction被设置成了row或者row-reverse的话，交叉轴的方向就是沿着列向下的。

![](_v_images/20200610140311284_9383.png)

如果主轴方向设成了 column或者 column-reverse，交叉轴就是水平方向.
![](_v_images/20200610140415979_20624.png)

## 3.起始线和终止线
flex模型不会对文档的书写模式提供假设。过去，css的书写模式主要被































































# 教学视频知识点
## 1.flex相关属性
![](_v_images/20200610175407178_23127.png)

### 1.flex-direction:     主轴方向,默认从左往右 
四个取值：
row    从左往右
row-reverse  从右往左
column  从上到下
column-reverse  从下往上
 ![](_v_images/20200611152943217_1179.png)

### 2.justify-content 在主轴上的对齐方式
justify-content属性用来使元素在主轴方向上对齐，主轴方向是通过 flex-direction 设置的方向。初始值是flex-start，元素从容器的起始线排列。
有以下几个取值：
stretch  :  伸展
flex-start:  从开始位置
flex-end :从结束位置
center:  在中间排列
space-around  :  使每个元素的左右空间相等。
space-between  :   把元素排列好之后的剩余空间拿出来，平均分配到元素之间，所以元素之间间隔相等
space-evenly :   可以平均item的间距

![](_v_images/20200611162929300_2806.png)

### 3.align-items
align-items决定了item在交叉轴上的对齐方式。
这个属性的初始值为stretch，这就是为什么flex元素会默认被拉伸到最高元素的高度。实际上，它们被拉伸来填满flex容器 —— 最高的元素定义了容器的高度。
![](_v_images/20200611211813388_5941.png)

### 3.flex-wrap  可以换行
flexbox内的item如果一行不够放的话，会进行压缩item,而不会自动换行
flex-wrap可以实现自动换行功能！

flex-wrap: nowrap   默认值，不会换行
flex-wrap:wrap    可以换行显示
flex-wrap:wrap-reverse    在交叉轴上进行反转














