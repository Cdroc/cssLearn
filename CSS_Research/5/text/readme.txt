相对长度单位   -- px -- 不同显示器的分辨率不同，每个像素的实际大小也不同。
               -- em -- 1em表示的长度是其父元素中字母m的标准宽度
               -- ex -- 1ex表示的长度是其父元素中字母x的标准高度
绝对长度单位   -- in -- inch，英寸
               -- cm -- centimeter，厘米
               -- mm -- millimeter，毫米
               -- pt -- point，印刷的点数，在一般的显示器中1pt相当于1/72inch
               -- pc -- pica，1pc=12pt
百分比长度单位 -- %  -- "font-size:200%"表示文字的大小为原来的两倍

-----------------------------------------------------------------------------

font-weight: normal; -- 正常
font-weight: bold;   -- 粗体

font-style: normal;  -- 正常
font-style: oblique; -- 倾斜
font-style: italic;  -- 意大利体

text-transform: capitalize; -- 单词首字大写
text-transform: uppercase;  -- 全部大写
text-transform: lowercase;  -- 全部小写

text-decoration: underline;    -- 下划线
text-decoration: overline;     -- 顶划线
text-decoration: line-through; -- 删除线
text-decoration: blink;        -- 闪烁（IE中无效）
text-decoration: underline overline line-through;    -- 同时拥有三种线

text-align: center;  -- 居中对齐
text-align: left;    -- 左对齐
text-align: right;   -- 右对齐
text-align: justify; -- 两端对齐

（text-indent: 2em; -- 段首缩进）

-----------------------------------------------------------------------------

first-letter.htm
line-height-1.htm
line-height-2.htm -- 行高的不同写法，显示情况也会发生变化
                  -- 缩写 -- font: 12px/18px Arial; -- 大小/行高 字体
                          -- font: 12px/1.5 Arial;  -- 大小/行高 字体
sigle-vertical.htm
multi-vertical.htm -- 竖直居中