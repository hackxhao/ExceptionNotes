### 当前环境
win+eclipse4.2

### 问题描述
在eclipse里启动tomcat的时候出现`Tomcat:Several ports (8005, 8080, 8009)`

![](http://webug.oss-cn-beijing.aliyuncs.com/imgBed/20190116043251931.png)



### 问题原因
8080端口被其他应用所占用,或者是正在启动了Tomcat的Eclipse非正常的关闭。 
### 修复过程
第一步：查看端口

![](http://webug.oss-cn-beijing.aliyuncs.com/imgBed/20190116043607443.png)

第二步：根据PID终止进程

![](http://webug.oss-cn-beijing.aliyuncs.com/imgBed/20190116043901468.png)

第三步：

重启tomcat


### 总结

在关闭eclipse的时候请注意，先停止tomcat服务
