## 通过Alist,Clouddrive2挂载夸克网盘到本地

### 启动项问题

按Win＋R

输入{% copy shell:startup %}

进入开机启动目录:C:\Users\用户名\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup

在其中建立文本文档，粘贴以下内容：

```cmd
cd C:\Users\saevio
alist server
```

重命名文件后缀为**.bat**

### Alist问题

不要下载官网windows版本,下载github版本

启动：Alist server

http://127.0.0.1:5244

账号:saevio

### 挂载到本地

使用**Raidrive**

配置如下：

![image-20230803181553972](https://article.biliimg.com/bfs/article/8299937a1ca2f4068eb01918cbace3049cbb80be.png)

