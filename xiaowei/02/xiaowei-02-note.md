## 小薇02
### 导航栏
-   显示效果为左对齐是logo，右对齐是居中菜单
-   要点
    -   给各个CSS定义加上`background`来帮助debug
    -   `line-height`定义行元素高，`height`定义其他元素高，包括块元素
    -   使用`float: right`实现右对齐
    -   `div`默认有margin，需要去掉
    -   定义元素为`inline`，使其作为行元素
    -   定义元素为`inline-block`，使其显示为行内元素，内部元素是块元素
    -   行元素定义`line-height`和`vertical-align`来实现对齐

### 伪类
-   例如`a`的伪类有如下四个：
    -   `a:link`未点击过的链接
    -   `a:visited`已点击过的链接
    -   `a:hover`悬停在链接上时
    -   `a:active`点击链接时
-   使用时有如下要点：
    -   CSS中定义伪类时顺序不能乱，因为后者定义的伪类会覆盖前者
    -   按上述顺序定义即可

### box加阴影
-   语法如下
    -   `{box-shadow:[inset] x-offset y-offset blur-radius spread-radiuscolor}`
    -   `x-offset`是X轴偏移
    -   `y-offset`是Y轴便宜
    -   `blur-radius`是阴影渐变半径
    -   `spread-radiuscolor`是渐变色
-   例如
    -   `box-shadow: 2px 2px 2px #444444`

### img-box实现
-   要点在于设置好`margin`,`padding`,`width`以及`border`
-   内部居中则设置`text-align`

### 标题前加竖线
-   用div包住header，给div增加padding
-   再给div增加`border-left: 5px solid #888888`

### 其他记录
-   ul去掉默认style，`list-style: none;`
-   button去掉阴影，`border:0;`
-   button增加圆角，`border-radius: 10px;`