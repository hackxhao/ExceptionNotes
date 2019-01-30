### 当前环境
Centos7.4 + docker

### 问题描述
在执行`docker run -d --name jenkins -p 9100:8080 -v /home/jenkins_home:/var/jenkins_home jenkins`命令时启动报错:

```java
touch: cannot touch '/var/jenkins_home/copy_reference_file.log': Permission denied
Can not write to /var/jenkins_home/copy_reference_file.log. Wrong volume permissions?
```

### 问题原因
挂载目录到宿主机时没有权限

### 修复过程

先查看容器用户
```java
docker run -ti --rm --entrypoint="/bin/bash" jenkins -c "whoami && id"
```

![](https://webug.oss-cn-beijing.aliyuncs.com/imgBed/20190130080049384.png)

然后将挂载到宿主机的目录进行赋权
```
chown -R 1000:1000 /home/jenkins_home
```
无任何则成功


### 总结
暂无
