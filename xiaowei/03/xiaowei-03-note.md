## 小薇03
### 思路一
-   先浮动左右两栏，中间一栏设置margin
    -   左栏，`float: left; width: 250px;`
    -   右栏，`float: right; width: 250px;`
    -   中间栏，`margin: 0 250px;`
-   HTML中顺序必须是左右栏先定义，中间栏最后定义
### 思路二
-   中间栏也浮动，左右栏左浮动，且使用负margin
    -   中间栏需要双重div
        -   父层`float: left; width: 100%;`
        -   子层`margin:0 250px;`
    -   左栏，`float: left; margin-left: -100%;`
        -   由于中间栏是全宽，所有-100% margin就相当于浮在最左
    -   右栏，`float: left; margin-left:-250px;`
        -   右栏相当于往左margin其宽度，也就相当于浮在最右   
-   HTML中顺序必须是中间栏首先定义，然后定义左右栏
### 小结
-   HTML中先后顺序意义在于以先定义的为基准进行定位

### 定位
-   static，默认定位
-   absolute，绝对定位，使用top down left right基于整个页面定位
    -   如果其父元素使用了relative相对定位，其会基于父元素的范围进行绝对定位   
-   relative，相对定位，可以使用top down left right基于其父元素定位

### 浮动
-   float，常用于多栏布局，也算是唯一手段，使其相对于前面的元素定位
-   clear，清除浮动