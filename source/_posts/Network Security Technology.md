---
title: 信息安全技术实验
cover: http://tva1.sinaimg.cn/mw690/008e1sKigy1h7or6ae8xaj31dd0rs7sn.jpg
---

分享下答案
<!-- more --><!-- more -->

# **信息扫描课程**

## 主机信息扫描 {% emoji blobcat blobcatalt %}

{% folding child:codeblock open:false 主机存活性探测实验 %}

上图4中，命令ping –n 6 100.100.0.26（目标机IP地址）的结果中可以看出扫描了____次。

【正确答案】：6

上图7中，Nmap工具中的-sS参数是TCP扫描类型中的（见图7覆盖位置，注意格式）

【正确答案】：TCP SYN

根据端口列表文件我们可以知道，上图17中覆盖位置（箭头处）端口7的信息是____（注意区分大小写）

【正确答案】：Echo

在Linux中Fping是以___的方式向列表中的所有IP地址发送ICMP报文回送请求。

【正确答案】：并行

则上图27中覆盖位置是____时，表明100.100.0.14主机是存活的（注意大小写格式）

【正确答案】：host up

BCDDB

{% endfolding %}

{% folding child:codeblock open:false 主机信息探测实验 %}

DDDDC

{% endfolding %}

{% folding child:codeblock open:false 端口服务探测实验 %}

ABDCA

{% endfolding %}

{% folding child:codeblock open:false 操作系统指纹探测实验 %}


【填空题】直接ping目标主机的时，数据包是默认发送了____个。（见图1覆盖箭头，请按标准填写）

【正确答案】：4

【填空题】使用nmap –O命令得到的系统指纹结果中，可以看到netbios-ssn服务所开启的端口是____（见图4覆盖处，请按标准填写）

【正确答案】：139

BCABD

{% endfolding %}

##  网络信息扫描 {% emoji blobcat ablobcatrainbow %}

{% folding child:codeblock open:false 路由信息探测实验 %}

DABB

{% endfolding %}

{% folding child:codeblock open:false 交换式网络嗅探实验 %}

【填空题】在设置过滤规则时，协议捕编辑是选项卡的第四个选项是____【见图15中覆盖部分】

【正确答案】：Advanced

【填空题】在进行对FTP数据捕获的结果中，可以看到USER用户名是____（见图29覆盖处，请按标准填写）

【正确答案】：test

{% endfolding %}

{% folding child:codeblock open:false 网络连通探测实验 %}

1【单选题】如上图3，ping 127.0.0.1时，发送数据为多少字节 ？

A. 32

B. 256

C. 64

D. 128

【正确答案】：C

ACDBD

{% endfolding %}

{% folding child:codeblock open:false 局域网信息探测实验 %}

【单选题】在定制扫描选项时，“General”选项卡中“Max.threads”最大可以取值为【 】

A. 500

B. 1000

C. 2000

D. 100

【正确答案】：B

DBDC

{% endfolding %}

{% folding child:codeblock open:false DNS域名信息探测实验 %}

DDABD

{% endfolding %}

{% folding child:codeblock open:false 网络注册信息探测实验 %}

使用whois.chinaz.com站长之家查询注册信息结果中，可以得到baidu的创建时间____（见图4覆盖处，请按标准填写）

【正确答案】：1999年10月11日

【填空题】使用whoistd工具查询注册信息结果中，可以得到的注册商Registrar是____（见图6覆盖处，请按标准填写）

【正确答案】：MarkMonitor, Inc.

DCABB

## 网络信息获取 {% emoji blobcat ablobcatwave %}

{% folding child:codeblock open:false 网站后台扫描wscan %}

{% endfolding %}

