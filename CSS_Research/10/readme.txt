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