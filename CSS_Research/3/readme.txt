1.盒子模型 -- 顺时针：上右下左(top right bottom left)
           -- content(内容) padding(内边距) border(边框) margin(外边距)
	   -- 控件宽高是相对于内容的（content -- width height）
    1.1属性值简写 -- border-width:1px;             -- 上右下左
                  -- border-width:1px 2px;         -- 上下 左右
		  -- border-width:1px 2px 3px;     -- 上 左右 下
		  -- border-width:1px 2px 3px 4px; -- 上 右 下 左
    1.2块级元素   -- block  -- div  -- 上下margin取较大的值
    1.3行内元素   -- inline -- span -- 左右margin取两者之和
    1.4嵌套       -- 各浏览器有所区别（IE自适应 FF按固定值显示）
