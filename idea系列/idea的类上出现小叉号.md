### 当前环境
win+idea 2017.3.1

### 问题描述
idea的类上面出现小叉号（X）类似于
![1.png](https://img-blog.csdn.net/20161020095631049?watermark/2/text/aHR0cDovL2Jsb2cuY3Nkbi5uZXQv/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70/gravity/Center)



### 问题原因
当前类不会在工程编译的时候进行编译
### 修复过程
ctrl+alt+s打开Settings设置查找excludes，
在右侧的Path中选中文件，删除，即可解决。

![1.png](http://webug.oss-cn-beijing.aliyuncs.com/imgBed/20190121105647884.png)


### 总结
暂无

