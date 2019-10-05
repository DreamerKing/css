网格布局
Grid Container 网格元素 所有网格元素的父容器
Grid Item 网格项
Grid Line 网格线 组成网格项的分界线
Grid Track 网格轨道 
Grid Cell 网格单元
Grid Area 网格区域

单位 
1. fr 剩余空间分配数
2. gr 网格数

+ Grid Container
1. display: grid|inline-grid|subgrid(浏览不兼容) 但元素设置网格布局之后，column、float、clear、vertical-align属性无效

2. grid-template -> grid-template-ro ws / grid-template-columns grid-template-areas
    + grid-template-columns: <track-size>|<line-name><track-size>
    + grid-template-rows: <track-size>|<line-name><track-size>
    + grid-template-areas:none|<grid-area-name>|.
3. gap
    + grid-column-gap
    + grid-row-gap
4. items
    + justify-items 行轴
    + aligin-items
    + place-items: column row
5. content
    + justify-content: space-aroud|space-between|space-evenly
    + align-contnent
    + place-content: 
6. grid-auto
    + grid-auto-columns
    + grid-auto-rows
    + grid-auto: row|column|dense
7. grid

CSS函数
1. repeat(repeat, value)
2. fit-content()
3. minmax(min, max)

网格
1. start/end: 
    + grid-column-start
    + grid-column-end
    + grid-row-start
    + grid-row-end
    + grid-column
    + grid-row
2. grid-area
3. self
+ justify-self
+ align-self 