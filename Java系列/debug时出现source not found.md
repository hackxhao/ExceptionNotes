### 当前环境
win+eclipse4.2

### 问题描述
在eclipse里debug项目时出现 `source not found`页面,但是断点的那个类明明存在。
![49dda335d66aba6e.png](http://www.tzr.me/images/2019/01/04/49dda335d66aba6e.png)

### 问题原因
资源包没有加载到
### 修复过程
第一步：

![1.png](http://www.tzr.me/images/2019/01/04/1.png)

第二步：

![2.png](http://www.tzr.me/images/2019/01/04/2.png)

第三步：

![3.png](http://www.tzr.me/images/2019/01/04/3.png)

点击OK 然后选中你的项目就行了，再调试的时候就可以跟踪断点到你的类中的。

### 总结
暂无


> 原文：https://www.cnblogs.com/programmer1/p/4411037.html