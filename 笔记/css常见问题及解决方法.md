#####  常见的问题
1. 打字错误或者语法错误:
* 选择带有自动补全功能的编辑器
* 用[css validator](http://jigsaw.w3.org/css-validator/)验证 *看清楚认真一些
2. 样式出不来
 * 样式层级被覆盖,提高样式的特殊性(!important)
 * 让一般更一般，让特殊更特殊,不要随意添加特殊的选择器
3. 外边距叠加的问题
 * 原因：元素没有边框或者内边距,它的高度就是所包含子元素顶部到底部边框之间的距离,子元素的外边距会突出显示到父元素的外边
 * 加个内边距或者加个边框(可查看 chrome devtool的elements视图)
4. ie的bug,尝试让元素拥有[布局](https://www.cnblogs.com/top5/archive/2011/06/30/2094044.html)
 * 条件注释
5. 明智地进行hack和使用过滤器(\*)
6. 设置为auto可将绝对定位的元素拉回原来的地方
*****
##### 怎么抓bug
1. 检查自己的html,css,检查打字错误和语法错误,确保浏览器以标准模式解析文档(DOCTYPE)
2. 从一开始就要避免bug的产生，使用尽可能简单的代码实现需求
3. 隔离问题：例子:给出现问题的元素加上边框或者轮廓,尝试修改css属性,看看它有什么变化,尝试一些常见的解决方案
4. 创建基本测试案例,提出有问题的html代码块,逐步注释css代码，直到留下有问题的css代码
5. 修复问题,而不是修复症状,例子:回避这个问题用另外的方案解决，实在回避不了，就把css规则过滤到一个单独的样式中,向浏览器提供支持
6. 请求帮助
 * 简洁的描述清楚问题的标题
 * 对问题进行简短的总结
 * 贴出基本的测试案例或者截图
