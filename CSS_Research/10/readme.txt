边框合并规则 -- hidden > ... > none
             -- 粗 > 细
             -- border-width相同时 -- double > solid > dashed > dotted > ridge > outset > groove > inset
             -- 仅颜色不同时 -- 单元格 > 行 > 行组 > 列 > 列组 > 表格
             -- IE6并不完全遵守上述规则

cellpadding在CSS中可用border-spacing代替，但IE6、IE7都不支持这个属性

表格宽度 -- table-layout -- fixed(固定方式)
                         -- auto(自动方式，默认)

summary
caption
thead tbody tfoot 
col -- 通过该标记可设置整列单元格的样式
    -- 要写成<col/>，不能写成<col></col>
    -- 只支持IE6、IE7
    -- 其他浏览器兼容方式，使用“邻接”选择器
    -- IE6不支持“邻接”选择器

-------------------------------------------------------

pretty-1-5.htm -- td+td+td “邻接”选择器 
               -- 表示每一行的第三个td为选中的元素

pretty-2.htm   -- IE6中tr标记不支持“:hover”伪类别
pretty-2-2.htm -- 添加.hover类别，通过js实现 