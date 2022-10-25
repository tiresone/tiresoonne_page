# 学习记录

## 一些符号

·
.a 是 class
#a 是 id

· css 中.a b c d 的格式是设置.a 下的所有 b，c，d 的格式。
而.a>b>c>d 格式才是设置.a 下 b 下 c 下的 d 的格式
这一点使我耗费了一个下午才实现下拉菜单栏

· 代码中任何细微的格式差别都可能有不同的含义

<!-- css各种标签的含义 -->

overflow

## 关于图片的居中

常用的块状元素：< div>< p>< h>< ol>< ul>< dl>< table>< address>< blockquote>< form>

常用的行内元素：< a>< span>< br>< i>< em>< strong>< label>< q>< cite>< code>< var>

常用的行内块状元素：< img > < imput >

块级元素指定：使用 text-align：center 就无效了。

如果需要设置居中，通过设置左右两边的 margin 值为“auto”来实现。

## 动效 transition(条件触发)

transition-property 是规定应用过渡的 CSS 属性的名称

transition-duration 定义过渡效果花费的时间。默认是 0 秒

transition-timing-function 规定过渡效果的时间曲线。默认是 ease

        linear 是以相同速度开始至结束的过渡效果

        ease 是从慢速开始，然后变快，然后慢速结束的过渡效果

        ease-in 是以慢速开始的过渡效果

        ease-out 是以慢速结束的过渡效果

        ease-in-out 是慢速开始和结束的过渡效果

transition-delay 规定过渡效果从何时开始，即是延时效果。默认是 0

transition 是连写格式：

        transition：过渡属性  过渡时长  运动速度 延迟时间

                       transition-property    transition-duration   transition-timing-function   transition-delay

## 动效 animation

css 里写

.类名 {
**position: relative;**
-webkit-animation: 动画函数名 5s infinite; /_Safari and Chrome_/
animation: 动画函数名 5s infinite;
}
@keyframes 动画函数名 {
from {
left: 0px;
}
to {
left: 200px;
}
}
@-webkit-keyframes 动画函数名 /_Safari and Chrome_/ {
from {
left: 0px;
}
to {
left: 200px;
}
}
