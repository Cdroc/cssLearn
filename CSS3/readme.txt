CSS3 边框 -- 能够创建圆角边框，向矩形添加阴影，使用图片来绘制边框
          -- border-radius -- 圆角边框
          -- box-shadow    -- 边框阴影 -- h-shadow -- 必需，水平阴影的位置，允许负值
                                       -- v-shadow -- 必需，垂直阴影的位置，允许负值
                                       -- blur     -- 可选，模糊距离
                                       -- spread   -- 可选，阴影的尺寸
                                       -- color    -- 可选，阴影的颜色
                                       -- inset    -- 可选，将外部阴影改为内部阴影
          -- border-image  -- 边框图片 -- border-image-source -- 用在边框的图片路径
                                       -- border-image-slice  -- 图片边框向内偏移
                                       -- border-image-width  -- 图片边框的宽度
                                       -- border-image-outset -- 边框图像区域超出边框的量
                                       -- border-image-repeat -- 图像边框是否平铺、铺满或拉伸
----------------------------------------------------------------------------------
CSS3 背景 -- background-size   -- 规定背景图片的尺寸
                                  -- 能够以像素或百分比规定尺寸
                                  -- 如果以百分比规定尺寸，那么尺寸相对于父元素的宽度和高度
          -- background-origin -- 规定背景图片的定位区域，backgroun-position属性相对于什么位置来定位
                                  -- 背景图片可以放置于content-box/padding-box/border-box区域
                                  -- padding-box -- 背景图像相对于内边距框来定位
                                  -- border-box  -- 背景图像相对于边框盒来定位
                                  -- centent-box -- 背景图像相对于内容框来定位
          -- background-image  -- 允许使用多个背景图像
          -- background-clip   -- 规定背景的绘制区域
                                  -- border-box  -- 背景被裁剪到边框盒
                                  -- padding-box -- 背景被裁剪到内边距框
                                  -- content-box -- 背景被裁剪到内容框
----------------------------------------------------------------------------------
CSS3 文本效果 -- text-shadow         -- 向文本添加阴影
              -- word-wrap           -- 允许对长的不可分割的单词进行分割并换行到下一行
              -- hanging-punctuation -- 规定标点符是否位于线框之外
              -- punctuation-trim    -- 规定是否对标点符进行修剪
              -- text-align-last     -- 设置如何对齐最后一行或紧挨着强制换行符之前的行
              -- text-emphasis       -- 向元素的文本应用重点标记以及重点标记的前景色
              -- text-justify        -- 规定当 text-align 设置为 "justify" 时所使用的对齐方法
              -- text-outline        -- 规定文本的轮廓
              -- text-overflow       -- 规定当文本溢出包含元素时发生的事情
              -- word-break          -- 规定非中日韩文本的换行规则
              -- text-wrap           -- 规定文本的换行规则
----------------------------------------------------------------------------------
CSS3 字体 -- @font-face {
                 font-family: name; -- 必需，规定字体的名称
                 src: url("x.ttf"), -- 必需，定义字体文件的url
                      url("x.eot"); /*IE9+*/
                 font-stretch: normal/condensed/ultra-condensed/extra-condensed/semi-condensed/
                               expanded/semi-expanded/extra-expanded/ultra-expanded;
                               -- 可选，定义如何拉伸字体，默认normal
                 font-style: normal/italic/oblique; -- 可选，定义字体样式，默认normal
                 font-weight: normal/bold/100/200/300/400/500/700/800/900;
                              -- 可选，定义字体粗细，默认normal
                 unicode-range: unicode-range; 
                               -- 可选，定义字体支持的UNICODE字符范围，默认"U+0-10FFFF"
             }
----------------------------------------------------------------------------------
CSS3 2D 转换 -- transform  -- 能够对元素进行移动、缩放、转动、拉长或拉伸
                           -- 使元素改变形状、尺寸和位置的一种效果
                           -- translate(dx, dy)            -- 元素从当前位置移动(单位px)
                           -- rotate(angle)                -- 元素顺时针旋转给定的角度(单位deg)
                           -- scale(sx, sy)                -- 元素的尺寸会增加或减少
                           -- skew(x-angle, y-angle)       -- 元素翻转给定的角度(单位deg)，斜拉
                           -- matrix(sx, 0, 0, sy, dx, dy) -- 把所有2D转换方法组合在一起

CSS3 3D 转换 -- transform  -- 使用3D转换对元素进行格式化
                           -- 使元素改变形状、尺寸和位置的一种效果
                           -- rotateX(angle) -- 元素围绕其X轴以给定的度数进行旋转(单位deg)
                           -- rotateY(angle) -- 元素围绕其Y轴以给定的度数进行旋转(单位deg)

CSS3 过渡    -- transition -- 元素从一种样式逐渐改变为另一种的效果
                           -- 规定希望把效果添加到哪个CSS属性上
                           -- 规定效果的时长
                           -- transition: width 2s, height 2s, transform 2s;
             -- transition-property        -- 规定应用过渡的CSS属性的名称
             -- transition-duration        -- 定义过渡效果花费的时间，默认0
             -- transition-timing-function -- 规定过渡效果的时间曲线，默认ease
             -- transition-delay           -- 规定过渡效果何时开始，默认0

CSS3 动画 -- @keyframes animation -- 使元素从一种样式逐渐变化为另一种样式的效果
                                  -- @keyframes name {
                                         // from {background: red;}
                                         // to {background: blue;}
                                         0%   {background: red;}
                                         50%  {background: green;}
                                         100% {background: blue;}
                                     }
                                     div {
                                         animation: name 5s;
                                     }
                                  -- from/to等同于0%/100%
          -- @keyframes                -- 规定动画
          -- animation                 -- 所有动画属性的简写属性，除了 animation-play-state 属性
          -- animation-name            -- 规定 @keyframes 动画的名称
          -- animation-duration        -- 规定动画完成一个周期所花费的秒或毫秒。默认是 0
          -- animation-timing-function -- 规定动画的速度曲线。默认是 "ease"
          -- animation-delay           -- 规定动画何时开始。默认是 0
          -- animation-iteration-count -- 规定动画被播放的次数。默认是 1
          -- animation-direction       -- 规定动画是否在下一周期逆向地播放。默认是 "normal"
          -- animation-play-state      -- 规定动画是否正在运行或暂停。默认是 "running"
          -- animation-fill-mode       -- 规定对象动画时间之外的状态
----------------------------------------------------------------------------------
CSS3 多列 -- 能够创建多个列来对文本进行布局，就像报纸那样
          -- column-count -- 规定元素应该被分隔的列数
          -- column-gap   -- 规定列之间的间隔
          -- column-rule  -- 规定列之间的宽度、样式和颜色规则
             -- column-rule-color -- 规定列之间规则的颜色
             -- column-rule-style -- 规定列之间规则的样式
             -- column-rule-width -- 规定列之间规则的宽度
          -- column-fill  -- 规定如何填充列
          -- column-span  -- 规定元素应该横跨的列数
          -- column-width -- 规定列的宽度
          -- columns      -- 规定设置column-width和column-count的简写属性
----------------------------------------------------------------------------------
CSS3 用户界面 -- 新的用户界面特性包括重设元素尺寸、盒尺寸以及轮廓等
              -- resize         -- 规定是否可由用户调整元素尺寸
              -- box-sizing     -- 允许以确切的方式定义适应某个区域的具体内容
              -- outline-offset -- 对轮廓进行偏移，并在超出边框边缘的位置绘制轮廓
                                -- 轮廓不占用空间
                                -- 轮廓可能是非矩形
              -- appearance     -- 允许您将元素设置为标准用户界面元素的外观
              -- icon           -- 为创作者提供使用图标化等价物来设置元素样式的能力
              -- nav-down       -- 规定在使用 arrow-down 导航键时向何处导航
              -- nav-index      -- 设置元素的 tab 键控制次序
              -- nav-left       -- 规定在使用 arrow-left 导航键时向何处导航
              -- nav-right      -- 规定在使用 arrow-right 导航键时向何处导航
              -- nav-up         -- 规定在使用 arrow-up 导航键时向何处导航