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

-----------------------------------------------------------------------

01 -- 对于groove/inset/outset/ridge,IE支持的不够理想,在实际制作网页的时候不推荐使用
03 -- 在给元素设置background-color背景色时，IE作用的区域为content + padding,
      而Firefox则是content + padding + border。
      IE中虚线空白的地方露出来的是padding部分的背景，
      而在Firefox中，虚线空白的地方露出来的是margin部分的背景。
   -- body是一个特殊的盒子，它的背景是会延伸到margin的部分，
      而其他盒子的背景色只会覆盖“padding+内容”部分（IE浏览器中），
      或者“border+padding+内容”部分（Firefox浏览器中）。
04 -- DOM -- Document Object Model -- 文档对象模型
   -- <meta charset="UTF-8" /> -- 防止中文乱码
09 -- 父子块的margin时，IE与Firefox处理情况不同
      父div高度小于子div的高度加上margin的值，IE浏览器会自动扩大，
      而Firefox不会，从CSS的标准规范来说，IE的这种处理方法是不合规范的。