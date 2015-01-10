background-color: repeat;    -- 沿水平和竖直两个方向平铺
background-color: no-repeat; -- 不平铺，即只显示一次
background-color: repeat-x;  -- 只沿水平方向平铺
background-color: repeat-y;  -- 只沿竖直方向平铺

background: gray url(bg.gif) repeat-x -- 背景样式属性缩写
         -- 背景色 背景图片 平铺方式

background-position: left;
background-position: right;
background-position: top;
background-position: bottom;
background-position: center; -- 可以设置两个值，缺省的为center

---------------------------------------------------------------

<h1><span> </span> Head Line </h1> -- 这对span标记没有实际的语义作用，仅作为一个CSS“钩子”，用于设置背景图像。然后通过对span元素使用绝对定位，将图像覆盖在文字的上面，这样即使关闭了CSS，仍然可以看到文本标题。这个方法的缺陷是，标题图像不能使用透明的图像，否则会露出文字。