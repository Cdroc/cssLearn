1.浮动 -- float -- 脱离标准流
    1.1设置浮动 -- float:left
                -- float:right
    1.2清除浮动 -- clear:left
                -- clear:right
                -- clear:both
2.定位 -- position -- top right bottom left相对于position才有意义
    2.1静态定位 -- static   -- 标准流     -- 未设置position则为static（含浮动）
    2.2相对定位 -- relative -- 标准流     -- 以原标准位置为基准偏移
    2.1绝对定位 -- absolute -- 脱离标准流 -- 以它的父标准框为基准偏移
                   （以最近的已设置定位属性的父框为标准框，都未设置，则为body）
    2.2固定定位 -- fixed    -- 脱离标准框 -- 以浏览器窗口为基准偏移（IE6不识别）
3.display属性   -- inline block none
