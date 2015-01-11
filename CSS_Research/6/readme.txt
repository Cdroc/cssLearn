a:link    -- 超链接的普通样式
a:visited -- 被点击过的超链接样式
a:hover   -- 鼠标指针经过超链接时的样式
a:active  -- 在超链接上单击时的样式（按下未弹起）

text-decoration:none -- 去掉下划线

a:link, a:visited {text-decoration: none;}
a:hover, a:active {text-decoration: underline;}
 -- 若交换上面两行代码的顺序，对鼠标指针经过时的设置将不会产生效果，这是由于“层叠”的原因，上面的这些CSS规则具有同样的特殊性，因此后面的规则将覆盖前面的规则，要按照上面的顺序来进行设置。
 -- a:link与a通常情况下是没区别的，但一个a标记没有设置跳转地址（即href属性）时，a:link的设置无效，而a的设置有效，所以在实际工作中，经常使用：
 a, a:visited {text-decoration:none;}
 而不用：
 a:link, a:visited{text-decoration:none;}

 --------------------------------------------------------------

 vertical.htm~vertical4.htm -- IE6中需要鼠标经过文字鼠标才有效果，需要在“navigation li a”中添加一条设置高度的CSS规则：height:1em;