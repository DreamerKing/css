相关书籍
《CSS设计指南》、《CSS权威指南》
# 相关概念 
+ 文档流(Normal FLow) 
+ 格式化上下文(Formatting Context)
+ 层叠上下文(Stacking Context)
+ 层叠水平(Stacking Level)
+ 层叠顺序(Stacking Order)

Formatting Context：指页面中的一个渲染区域，并且拥有一套渲染规则，他决定了其子元素如何定位，以及与其他元素的相互关系和作用。

BFC：块级格式化上下文，它是指一个独立的块级渲染区域，只有Block-level BOX参与，该区域拥有一套渲染规则来约束块级盒子的布局，且与区域外部无关。

BFC的生成：(满足其一即可)
+ 根元素
+ float的值不为none
+ overflow的值不为visible
+ display的值为inline-block、table-cell、table-caption
+ position的值为absolute或fixed

BFC的约束规则
+ 生成BFC元素的子元素会一个接一个的放置。垂直方向上他们的起点是一个包含块的顶部，两个相邻子元素之间的垂直距离取决于元素的margin特性。在BFC中相邻的块级元素外边距会折叠。
+ 生成BFC元素的子元素中，每一个子元素做外边距与包含块的左边界相接触，（对于从右到左的格式化，右外边距接触右边界），即使浮动元素也是如此（尽管子元素的内容区域会由于浮动而压缩），除非这个子元素也创建了一个新的BFC（如它自身也是一个浮动元素）。