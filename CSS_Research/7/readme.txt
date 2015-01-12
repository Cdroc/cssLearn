margin: 0 auto;   -- 水平居中
first-child       -- CSS伪类 -- IE不支持
overflow: hidden; -- 防止溢出（将溢出部分隐藏起来）
height: auto;     -- 高度自适应内容

-------------------------------------------------------------------------

vertical-border-1.htm -- IE上有bug，在“#menu a,#menu a:visited"的CSS规则里添加 height:1em;
bevel-navi.htm        -- line-height能使文字竖直居中显示，而height使文字竖直方向靠上对齐
arrow-navi.htm        -- overflow: hidden; -- 防止IE溢出
                      -- 在“#menu a,#menu a:visited"添加 width: 130px; -- 修复IE的bug
                      -- height: auto; -- 高度自适应内容