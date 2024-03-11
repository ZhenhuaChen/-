### 1. CSS选择器及其优先级
对于选择器的优先级：!important > 内联样式 > id选择器 > 类选择器、伪元素选择器、属性选择器 > 标签选择器
### 2. display：none和visibility：hidden的区别
在渲染树中display设置为none会让元素完全从渲染树中消失，渲染时不会占据任何空间。而visibility属性设置为hidden不会让元素从渲染树中消失，渲染的元素还是会占据相应的空间，只是内容不可见。
### 3. CSS的盒模型
CSS3的盒模型有两种：标准盒模型和IE盒模型<br />
盒模型都是由四个部分组成，分别是margin、border、padding和content<br />
- 标准盒模型的width和height属性的范围只包含了content
- IE盒模型的width和height属性的范围包含了border、padding和content<br />
可以通过修改元素的box-sizing属性来改变元素的盒模型：<br />
- box-sizing属性设置为content-box表示标准盒模型
- box-sizing设置为border-box表示IE盒模型
### 4. CSS sprites（雪碧图/精灵图）
CSS Sprites也就是雪碧图，将一个页面涉及到的所有图片都包含到一张大图中去，然后利用CSS的 background-image，background-repeat，background-position属性的组合进行背景定位。
- 优点：利用雪碧图​能很好地减少网页的http请求，从而大大提高了页面的性能；同时雪碧图能减少图片的大小。
- 缺点：作图麻烦，在图片合并时，要把多张图片有序的、合理的合并成一张图片，还要留好足够的空间，防止板块内出现不必要的背景。在宽屏及高分辨率下的自适应页面，如果背景不够宽，很容易出现背景断裂。开发的时候需要测量准确的位置，后期维护麻烦。

### 5. CSS的BFC
BFC也就是块格式化上下文
块格式化上下文（Block Formatting Context，BFC）是Web页面的可视化CSS渲染的一部分，是布局过程中生成块级盒子的区域，也是浮动元素与其他元素的交互限定区域。

通俗来讲：BFC是一个独立的布局环境，可以理解为一个容器，在这个容器中按照一定规则进行物品摆放，并且不会影响其它环境中的物品。如果一个元素符合触发BFC的条件，则BFC中的元素布局不受外部影响


### 5. css优化和提高性能的方法
