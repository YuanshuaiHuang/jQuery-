# jQuery-
一些为了辅助学习jQuery的小实例
##引言##
在原生JavaScript当中，当我们要操作HTML元素时，有三种方式可以找到这、目标元素：

 - 通过 id 找到 HTML 元素——document.getElementById("xxx")
 - 通过标签名找到 HTML 元素——document.getElementsByTagName("xxx")
 - 通过类名找到 HTML 元素——document.getElementsByClassName("xxx")

区分变量分别时元素的id、标签名、类名

那么在jQuery中我们是如何找到目标元素的呢？有没有更多，更简捷的方式呢？

##jQuery选择器##


挑一些比较常用的来讲解，其余的请大家查看
http://www.w3school.com.cn/jquery/jquery_ref_selectors.asp

###1、从JavaScript继承而来###

 - $("#XXX") —— 按ID查找
 - $(".XXX") —— 按类名查找
 - $("XXX") —— 按标签查找

###2、按聚合中的索引查找（辅助查找）###

 - $(":first") —— 第一个元素（索引为0）
 - $(":last") —— 最后一个元素（索引为length-1）
 - $(":odd") —— 奇数元素（索引为奇数）
 - $(":even") —— 偶数元素（索引为奇数）
 - $(":eq(n)") —— 指定索引（有点数组的意思）
 - $(":gt(n)") —— 大于某索引的元素（>n）
 - $(":lt(n)") —— 小于某索引的元素（<n）

###3、特殊查找###

 - $(":contains('XXX')") —— 含有指定字符串的元素
 - $("[href]") —— 含有某属性的元素

	延伸：
	$("[href='#']") —— 属性值等于限定
	$("[href！='#']") —— 属性值不等于限定
	$("[href^='#']") —— 属性值开头限定
	$("[href$='#']") —— 属性值结尾限定
	$("[href*='#']") —— 属性值包含限定(非严格要求)
	$("[href~='#']") —— 属性值包含限定(严格要求)

 - $("[href]") —— 含有某属性的元素
 - $(":empty") —— 无子（元素）节点的所有元素 （这里会有换行内容的干扰）
 - $(":hidden") —— display:none的情况
 - $(":visible") —— 除display:none以外的情况

###4、组合查找###

在这里说几个典型的：

 - $(".XXX #XXX") —— 类和ID选择搭配
 - $("XX:XX") —— 标签和辅助查找搭配
 - $("XX[XX]") —— 标签和属性查找搭配
 
 ...等等 大家可以根据实际需求自己探索


##一些小例子##

一些相关的小例子我已经写在DEMO中，欢迎大家访问并给出修改意见！

如果喜欢，不妨给出你的Star～

未完待续。

	
	
   	
