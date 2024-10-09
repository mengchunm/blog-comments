---
title: 信息安全技术实验
cover: https://article.biliimg.com/bfs/article/6ec68559496675b3983e6f03912594bd64587936.jpg
---

分享下答案
<!-- more --><!-- more -->

<meta name="referrer" content="no-referrer">


# <font color='red'> 该实验会记录时长，建议先完成至综合测验部分（中途不需要挂在网页后台），一段时间后再写实验总结</font>

## 实验1{% emoji blobcat ablobcatwave %}

### 信息扫描课程

#### 主机信息扫描 

https://mengchunm.github.io/font

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

####  网络信息扫描 

{% folding child:codeblock open:false 路由信息探测实验 %}

DABB

{% endfolding %}

{% folding child:codeblock open:false 交换式网络嗅探实验 %}

【填空题】在设置过滤规则时，协议捕编辑是选项卡的第四个选项是____【见图15中覆盖部分】

【正确答案】：Advanced

【填空题】在进行对FTP数据捕获的结果中，可以看到USER用户名是____（见图29覆盖处，请按标准填写）

【正确答案】：test

CDADB

{% endfolding %}

{% folding child:codeblock open:false 网络连通探测实验 %}

【单选题】如上图3，ping 127.0.0.1时，发送数据为多少字节 ？

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

{% endfolding %}

#### 网络信息获取 

{% folding child:codeblock open:false 网站后台扫描 %}

【填空题】wscan完成扫描后，在扫描结果中可以找到到地址http：//100.100.0.6/admin.asp?action=____（见图6覆盖处，请按标准填写）

【正确答案】：login

BDBCA

{% endfolding %}

{% folding child:codeblock open:false 综合扫描（X-scan）实验 %}

【填空题】在X-scan端口配置的预设知名服务端口中，pop3的端口号为____（见图12覆盖处，请按标准提填写）

【正确答案】：110

【填空题】在X-scan扫描结果报告中，可以看到漏洞“SMB运行在445端口”的风险等级是____（见图18覆盖处，请按标准填写）

【正确答案】：中

BCADD

{% endfolding %}

{% folding child:codeblock open:false 综合扫描（Nessus）实验 %}

【填空题】在新建扫描模板时，扫描类型Type为Run Now、Scheduled和____（见图26覆盖处，请按标准填写）

【正确答案】：Template

BAADD

{% endfolding %}

{% folding child:codeblock open:false Wireshark抓包实验 %}

【填空题】在抓包过程中，深蓝色的数据报文为____（见步骤1.5文字解释，请按标准填写）

【正确答案】：DNS

DCBCB

{% endfolding %}

{% folding child:codeblock open:false Wireshark工具的使用与TCP数据包分析实验 %}

【填空题】 FTP协议的抓包中，操作机发送请求时的信息是pass____，表示操作机以发送pass命令。（见图9覆盖处，请按标准填写）

【正确答案】：123456

CBDAC

{% endfolding %}

{% folding child:codeblock open:false 手工信息收集1 %}

【填空题】当一个搜索蜘蛛访问一个站点时，它会首先检查该站点根目录下是否存在____（答案见步骤1.1，请按标准填写）

【正确答案】：robots.txt

【填空题】发现网站有.git目录，重塑网页代码用到的工具是____（请按标准填写，注意大小写）

【正确答案】：GitHack

AABDD

{% endfolding %}

{% folding child:codeblock open:false 手工信息收集2 %}

我也不会，哈哈

{% endfolding %}

{% folding child:codeblock open:false 工具扫描 %}

【填空题】hydra指定扫描用户名的参数是____（注意使用英文字符，注意大小写）

【正确答案】：-l

【填空题】BurpSuite的默认监听（拦截）端口为____

【正确答案】：8080

DCB

{% endfolding %}

{% folding child:codeblock open:false 信息收集 %}

【单选题】从哪可以搜集到网站相关信息

A. LOGO

B. 标题

C. 版权所有

D. A、B、C

【正确答案】：D

DBACD

{% endfolding %}

### 漏洞扫描课程

#### 系统漏洞扫描

{% folding child:codeblock open:false 系统漏洞探测（Fluxay）实验 %}

【填空题】在高级扫描设置界面中，可以看到目标系统可以设置为ALL、Windows NT/2000、____（见图5覆盖处，请按标准填写）

【正确答案】：Linux/Unix

【填空题】在对FTP主机中的所有name设置扫描时，扫描的主机类型有POP3、FTP、NT/98、IIS/FRONT PAGE和____（见图13覆盖处，请按标准填写）

【正确答案】：SQL

DBCA

{% endfolding %}

{% folding child:codeblock open:false 利用retina探测系统弱点实验 %}

DADBA

{% endfolding %}

{% folding child:codeblock open:false Serv-U目录遍历漏洞扫描实验 %}

【填空题】在Nessus中添加新的扫描策略时，setting type有Basic、Port Scanning、Performance、Advanced四种。（见图6覆盖处，请按标准填写）

【正确答案】：Port Scanning

【填空题】在查看“Ftpfiles.txt”文件时，可以得到文件内容为：This is a ftp site test file!（见图18覆盖处，请按标准填写）

【正确答案】：ftp

AAADB

{% endfolding %}

#### 网站漏洞扫描

{% folding child:codeblock open:false 网站漏洞扫描（Wapiti）实验 %}

【填空题】示例XSS漏洞是以什么HTTP方法传递参数的GET（填写“GET”或“POST”，注意大小写）

【正确答案】：GET

CCCD

{% endfolding %}

{% folding child:codeblock open:false Iiswrite漏洞扫描实验 %}

【填空题】在查看目标机网站漏洞时，右键可以看到选项有Visit web(浏览网站)、Put file（上传文件）、Export（导出列表）和Delete（见图4覆盖处，请按标准填写）

【正确答案】：Delete

【填空题】试验中禁止webda后，再次用iisputscanner扫描网站时，就看不到该漏洞了，说明漏洞已经修补成功，其中扫描结果“PUT”状态为NO（见图16覆盖处，请按标准填写）

【正确答案】：NO

DACA

{% endfolding %}

{% folding child:codeblock open:false 网站漏洞扫描（owasp-zap）实验 %}

【填空题】
查看owasp zap工具的编码/解码功能时，当输入 “basic”该字符的md5哈希值为F17AAABC20BFE045075927934FED52D2（见图16覆盖处，请按标准填写）

【正确答案】：F17AAABC20BFE045075927934FED52D2

BCCD

{% endfolding %}

{% folding child:codeblock open:false 网站漏洞扫描（Vega）实验 %}

【填空题】选择的默认扫描模块中是否包含扫描XSS漏洞的模块是（ 回答“是”或“否”）

【正确答案】：是

BDBD

{% endfolding %}

{% folding child:codeblock open:false 综合漏洞探测（Nessus）实验 %}

【填空题】在Nessus中添加新的扫描策略时，setting type有Basic、Port Scanning、Performance、Advanced四种。（见图5覆盖处，请按标准填写）

【正确答案】：Performance

ADABCA

{% endfolding %}

{% folding child:codeblock open:false AWVS工具收集 %}

ACBAC

{% endfolding %}

{% folding child:codeblock open:false APPSCAN信息收集 %}

【填空题】本次爬区页面使用的扫描模式是（填写“完全扫描”或“仅探索”或“仅测试”）仅探索

【正确答案】：仅探索

CCB

{% endfolding %}

{% folding child:codeblock open:false BurpSuite信息收集 %}

BBACD

{% endfolding %}

## 实验2{% emoji blobcat ablobcatrainbow %}

### KALI应用课程

#### kalli信息收集

{% folding child:codeblock open:false Kali-安全渗透测试一般流程实验 %}

CBBDD

{% endfolding %}

{% folding child:codeblock open:false Kali-信息搜集之GoogleHack实验 %}

ABDC

{% endfolding %}

{% folding child:codeblock open:false Kali-信息搜集之目标获取实验 %}

【填空题】使用 Dig 命令对163.com进行测试时，AUTHORITY SECTION 的type类型是 SOA （见图6覆盖处，请按标准填写）



【正确答案】：SOA

【填空题】在使用dnsenum对163.com进行测试时，其结果中主机地址（Host’s addresses）信息的类型是 A （见图13覆盖处，请按标准填写）



【正确答案】：A

DBDC

{% endfolding %}

{% folding child:codeblock open:false Kali-信息搜集之主机探测实验 %}

【填空题】使用命令dmitry 163.com，查看其网站的端口信息时，可以得到其网站的80端口状态为 open （见图11覆盖处，请按标准填写）



【正确答案】：open

【填空题】使用wafw00f www.baidu.com 命令查看waf防护时，其结果中出现 “the site http：//www.baidu.com seems to be behind a WAF”,表明存在waf产品防护。（见图14覆盖处，请按标准填写）



【正确答案】：behind

CDDA

{% endfolding %}

{% folding child:codeblock open:false Kali-信息搜集之主机扫描实验 %}

【填空题】nmap扫描结果中，21端口的服务SERVICE是 ftp （见图14覆盖处，请按标准填写）



【正确答案】：ftp

CCCB

{% endfolding %}

{% folding child:codeblock open:false Kali-信息搜集之指纹识别实验 %}

【填空题】以telnet 命令连接端口进行探测时，结果中可以看出ftp服务器软件及版本信息为：FileZilla Server version 0.9.46 beta（见图2覆盖处，请按标准填写）.



【正确答案】：FileZilla

【填空题】在查看p0f截取的数据时，可以得到其参数params= none（见图8覆盖处，请按标准填写）



【正确答案】：none

DDCC

{% endfolding %}

{% folding child:codeblock open:false Kali-信息搜集之协议分析实验 %}

【填空题】使用命令sslscan www.alipay.com 查看支付宝证书信息时，结果中Testing SSL server www.alipay.com on port 443是测试SSL服务器使用的端口号（见图10覆盖处，请按标准填写）



【正确答案】：443

CABD

{% endfolding %}

#### Kali漏洞分析

{% folding child:codeblock open:false Kali- 漏洞分析之OpenVAS安装实验 %}

DDBA

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之OpenVAS使用实验 %}

【填空题】查看漏洞结果中远程攻击目标有http：//100.100.0.15/vicnum/ test.php （见图19覆盖处，请按标准填写，IP以实际实验为准）



【正确答案】：test.php

DBDD

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之扫描工具实验 %}

【填空题】使用lynis命令查看系统信息时，其结果中报告版本Report Version为 1.0（见图10覆盖处，请按标准填写）



【正确答案】：1.0

【填空题】在漏洞检测结果中，可以得到记录的主机名Assuming the OS is是linux（见图12覆盖处，请按标准填写）



【正确答案】：linux

DBBC

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之WEB爬行实验 %}

【填空题】在对目标机进行dirb命令进行目录扫描结果中，其列表文件位置为WORDLIST_FILES:/usr/share/dirb/ wordlists/common.txt（见图10覆盖处，请按标准填写）



【正确答案】：wordlists

【填空题】工具Vega的扫描漏洞结果中，可以看到SQL注入漏洞中http：//100.100.0.16/ WackoPicko/users/login.php的Method为POST（见图22覆盖处，请按标准填写，IP以实际实验为准）



【正确答案】：POST

DACD

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之WEB漏洞扫描（一）实验 %}

【填空题】可以看到目标机DavTestDir_sg28HqTdwIX6bG文件中新上传的文件后缀为asp、 aspx、cfm、cgi、html、jhtml、jsp、php、pl、shtml、txt。（见图10覆盖处，请按标准填写）



【正确答案】：aspx

【填空题】使用 “--version”的命令结果中，可以得到其版本为0.2 （见图13覆盖处，请按标准填写）



【正确答案】：0.2

【填空题】全面扫描结果中，可以看到其扫描方法Method为GET（见图23覆盖处，请按标准填写）



【正确答案】：GET

CABDCD

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之WEB漏洞扫描（二）实验 %}

【填空题】关于joomscan结果中可以看到，joomscan版本 0.0.7？。（见图4覆盖处，请按标准填写）



【正确答案】：0.0.7



【填空题】在浏览器中查看报告信息，可以得到发现的漏洞数目为4（见图30覆盖处，请按标准填写）



【正确答案】：4

DDCB

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之数据库评估（一）实验 %}

【填空题】破解成功后，可以看到目标服务器的用户名为 root，密码为hongya。（见图13覆盖处，请按标准填写）



【正确答案】：root

CDDD

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之数据库评估（二）实验 %}

【填空题】查看版本信息是，可以得到目标操作系统为32位（见图2覆盖处，请按标准填写）



【正确答案】：32

【填空题】请将图12中覆盖处的内容写出来mysql（见图14中覆盖处，请按标准填写）



【正确答案】：mysql

【填空题】请将图中覆盖处的内容写出来V4FP（见图17中覆盖处，请按标准填写）



【正确答案】：V4FP

CBDD

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之Web应用代理实验 %}

【填空题】Burp拦截结果中，可以看到其Accept-Language为en- US，en；q=0.5。（见图7覆盖处，请按标准填写）



【正确答案】：US

【填空题】报告结果中可以看到中等警报Medium个数为 3 （见图26覆盖处，请按标准填写）



【正确答案】：3

DBCDB

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之BurpSuite实验 %}

【填空题】在burp拦截的数据中，看可以看到登陆请求数据包的投递地址为http：//100.100.0.36/admin/ login .asp（见图10覆盖处，请按标准填写）



【正确答案】：login

【填空题】破解结果中， 可以看到密码为qwerasdf的状态状态Status是302 ，其返回长度不同于其他返回数据包，很有可能是猜解出来的密码。（见图19覆盖处，请按标准填写）



【正确答案】：302

【填空题】成功登录后台管理后，点击分类管理，可以看到有三个模块：大类管理、小类管理、 类别转移（见图22覆盖处，请按标准填写）



【正确答案】：类别转移

DCDDD

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞分析之Fuzz工具实验 %}

DACBD

{% endfolding %}

#### Kali密码攻击

{% folding child:codeblock open:false Kali- 密码攻击之在线攻击工具实验 %}

【填空题】使用findmyhash破解密码结果中可知结果为 1（见图12覆盖处，请按标准填写）



【正确答案】：1

【填空题】命令破解ssh的结果中，可以得到目标机100.100.0.16的用户名:root，密码：123456，其服务是ssh，端口为22（见图20覆盖处，请按标准填写）



【正确答案】：22


【填空题】在medusa暴力破解结果中，可以得到User：root，password： 123456（见图22覆盖处，请按标准填写）



【正确答案】：123456

【填空题】枚举结果中可以得到其candidate为“123456”，size为30（见图33覆盖处，请按标准填写）



【正确答案】：30

DDDCCB

{% endfolding %}

{% folding child:codeblock open:false Kali-密码攻击之离线攻击工具（一）实验 %}


【填空题】创建结果中可以看到生成659TB大的文件，一共有 66155263819776 行。（见图3覆盖处，请按标准填写）



【正确答案】：66155263819776


【填空题】破解结果中可以看出，哈希值d111b38c0e73bc867c4bad4023606a0e0df64c2f的原文密码为 password01 （见图19覆盖处，请按标准填写）



【正确答案】：password01


【填空题】判断结果中，可以得到哈希值2132f297a5a7a5a743894a0e4a801fc3的加密方式可能为MD2 、MD5、MD4、Double MD5等。（见图22覆盖处，请按标准填写）



【正确答案】：MD2


【填空题】从输出的信息中，可以看到6bcec2ba2597f089189735afeaa300d4哈希值可能是使用MD5加密的。（见图25覆盖处，请按标准填写）



【正确答案】：MD5


【填空题】查看破解结果，可以看到John成功破解了1个账户密码，其用户名为 root，密码为123456。（见图30覆盖处，请按标准填写）



【正确答案】：root


【填空题】破解结果中，可以看到一个账户密码破解成功，即User：root，Password： 123456（见图34覆盖处，请按标准填写）



【正确答案】：123456

CCCBDA

{% endfolding %}

{% folding child:codeblock open:false Kali-密码攻击之离线攻击工具（二）实验 %}


【填空题】结果中可以得到哈希值：ab56b4d92b40713acc5af89985d4b786的 破解结果是 abcde（见图覆盖处，请标准填写）



【正确答案】：abcde


【填空题】实验中正确载入哈希值之后，可以看到LM Pwd2为empty（见图11覆盖处，请按标准填写）



【正确答案】：empty

【填空题】破解成功后，可以按到LM Pwd 1是 123456 （见图12覆盖处，请按标准填写）



【正确答案】：123456

DECD

{% endfolding %}

{% folding child:codeblock open:false Kali-密码攻击之哈希传递攻击实验 %}


【填空题】从返回的哈希值中可以看到第一个用户为 Administrator（见图4覆盖处，请按标准填写）



【正确答案】：Administrator

EDAD

{% endfolding %}

{% folding child:codeblock open:false Kali-无线安全分析工具实验 %}

EDCB

{% endfolding %}

#### Kali漏洞利用

{% folding child:codeblock open:false Kali-漏洞利用之检索与利用实验 %}


【填空题】在相关的漏洞描述中， 可以看到mssql7.0的远程DOS漏洞路径为：/usr/share/exploitdb/platforms/./windows/dos/ 562图4覆盖处，请按标准填写）



【正确答案】：562

ADBD

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞利用之Metasploit基础实验 %}


【填空题】在预配置模块中，可以看到模块有auxiliary、exploit、payload和post（见图6覆盖处，请按标准填写）



【正确答案】：post


【填空题】目标机访问`http://100.100.0.15:8080/EXxX3ns4`时，查看其PDF内容为：Hello World !（见图23覆盖处，请按标准填写）



【正确答案】：World

DACADD

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞利用之Meterpreter介绍实验 %}

【填空题】show命令的使用说明结果中，可以得到其可用的模板有all,encoders,nops,exploits,payloads,auxiliary,plugins,info,options.（见图5覆盖处，请按标准填写）



【正确答案】：payloads


【填空题】使用命令“sysinfo”查看系统信息时，可以得到目标机OS信息 3.10.0 （见图14覆盖处，请按标准填写）



【正确答案】：3.10.0

ABDDDC

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞利用之Metasploit渗透测试实验 %}

DEAB

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞利用之BeEF实验 %}

【填空题】结果中可以看到beef主页检测到在线主机IP为127.0.0.1（即本机），点击右边“Details”查看详细信息，可以知道其浏览器版本Browser Version为 31（见图4覆盖处，请按标准填写）



【正确答案】：31

【填空题】实验发起攻击后，可以看到返回值为hongyaa，攻击成功。（见图7覆盖处，请按标准填写）



【正确答案】：hongyaa


【填空题】进入配置文件查看到其中的pass这是与metasploit通信约定的密码，其默认为 abc123（见图16覆盖处，请按标准填写）



【正确答案】：abc123

BADBB

{% endfolding %}

{% folding child:codeblock open:false Kali-漏洞利用之SET实验 %}

【填空题】点击查看登陆记录，可以看到其PersistentCookie状态为 yes（见图9覆盖处，请按标准填写）



【正确答案】：yes

BABABD

{% endfolding %}

#### Kali权限维持

{% folding child:codeblock open:false Kali-嗅探欺骗与中间人攻击实验 %}


【填空题】其配置完成页面中，可以看到信息GROUP 2：ANY (all the hosts in the list)（见图8覆盖处，请按标准填写）



【正确答案】：ANY


【填空题】目标机登陆后，操作机中得到信息DHCP：【FA:16:3E:4E:93:4C】REQUEST 100.100.0.8（见图10覆盖处，请按标准填写，目标IP及MAC地址以实验为准）



【正确答案】：REQUEST

BCCDC

{% endfolding %}

{% folding child:codeblock open:false Kali-权限维持之后门实验 %}


【填空题】可以看到webshell的代码已经被处理过，其代码为$b=strrev(“edoced_4”. 6esab”)。（见图2覆盖处，请按标准填写）



【正确答案】：6esab

【填空题】连接成功后，使用whoami命令查看目标机操作用户是，其结果为www-data（见图5覆盖处，请按标准填写）



【正确答案】：www-data


【填空题】连接端使用命令whoami查看用户，可以看到其结果为root（见图7覆盖处，请按标准填写）



【正确答案】：root

DBCD

{% endfolding %}

{% folding child:codeblock open:false Kali-权限维持之Tunnel实验 %}

ADDD

{% endfolding %}

#### Kali测试分析

{% folding child:codeblock open:false Kali-逆向工程工具实验 %}

DABBDC

{% endfolding %}

{% folding child:codeblock open:false Kali-压力测试工具实验 %}


【填空题】使用inviteflood进行攻击是可以看到用到目标主机的端口为 5060 （见图1覆盖处，请按标准填写）



【正确答案】：5060

【填空题】结果可以看到其攻击是将4569端口从4569端口泛洪10000次。（见图2覆盖处，请按标准填写）



【正确答案】：4569

DDCDC

{% endfolding %}

{% folding child:codeblock open:false Kali-数字取证工具实验 %}


【填空题】显示的测试项目结果中，可以看到其路径有/usr/sbin/chkrootkit（见图4覆盖处，请按标准填写）



【正确答案】：sbin


【填空题】文件信息中可以看到文件VistaSP0x64适用于Windows Vista SP0 x64。（见图7覆盖处，请按标准填写）



【正确答案】：SP0


【填空题】计算aaa的档案结果中，可以得到结果e4773f6627362b74b185fa03ce37783a *aaa（见图12覆盖处，请按标准填写）



【正确答案】：*aaa

BCDCD

{% endfolding %}

{% folding child:codeblock open:false Kali-报告工具与系统服务实验 %}


【填空题】在查看主机开放端口时，可以看目标机开通了21端口，其服务server为ftp （见图11覆盖处，请按标准填写）



【正确答案】：ftp


【填空题】扫描完成后可以看到目标机端口25的服务SERVICE为 smtp（见图18覆盖处，请按标准填写）



【正确答案】：smtp

BDBDCA

{% endfolding %}

## 实验3{% emoji blobcat ablobcatattentionreverse %}

### 密码破解课程

#### 本地密码破解

{% folding child:codeblock open:false Windows2003密码破解实验 %}


【填空题】请写出导出的本地密码散列文件的散列值是____（见图13覆盖处，请按标准填写）

【正确答案】：12BE6

【填空题】请使用SAMInside工具破解Windows本地密码散列文件得到的密码写出来是____（见图20覆盖处，请按标准填写）

【正确答案】：8967584106754

ADAB

{% endfolding %}

{% folding child:codeblock open:false WindowsXP密码破解实验实验 %}


【单选题】以下哪个是破解出来“test”用户的密码？

A. 8967584106754

B. 896758410675

C. 9867584106754

D. 9867584106755

【正确答案】：A

ADD

{% endfolding %}

{% folding child:codeblock open:false Windows7系统本地密码破解实验 %}

【填空题】请将使用PwDump7获取的用户散列值结果写出来____（见图9覆盖处，请按标准填写）

【正确答案】：AD44

【填空题】请将使用ophcrack工具破解散列值过程中，成功添加彩虹表后“Status”结果写出来____（见图15覆盖处，请按标准填写）

【正确答案】：on disk

ABD

{% endfolding %}

{% folding child:codeblock open:false Windows系统密码本地查看实验 %}

【填空题】请将上述被遮盖的查看结果进行写出来____（见图8覆盖处，请按标准填写）

【正确答案】：123456

【填空题】请将上述被遮盖的查看结果进行写出来____（没错，和上题一模一样）

【正确答案】：123456

ADAB

{% endfolding %}

{% folding child:codeblock open:false Salt型密码散列本地破解实验 %}

【填空题】请将简单模式的破解结果写入____（见图7覆盖处，请按标准填写）

【正确答案】：1resu

【填空题】请将字典模式的破解结果写入____（见图8覆盖处，请按标准填写）

【正确答案】：just4me

【填空题】请将暴力模式的破解结果写入 ____

【正确答案】：38947829

DDDC

{% endfolding %}

{% folding child:codeblock open:false Linux系统本地密码破解实验 %}

【填空题】请将上述被遮盖的破解结果进行写出来____（见图8覆盖处，请按标准填写）

【正确答案】：$6$6VM

【填空题】请将上述被遮盖的破解结果进行写出来____（见图10覆盖处，请按标准填写）

【正确答案】：adminuser

【填空题】请将上述被遮盖的破解结果进行写出来____（见图11覆盖处，请按标准填写）

【正确答案】：testpass

【填空题】请将上述被遮盖的破解结果进行写出来____（见图13覆盖处，请按标准填写）

【正确答案】：27861

CDBA CDBD

{% endfolding %}

#### 远程密码破解

{% folding child:codeblock open:false 网络服务远程密码破解(Brutus)实验 %}

【填空题】请将Brutus破解 POP3密码后的结果写入591（见图4覆盖处，请按标准填写）

【正确答案】：591

【填空题】使用Bruter破解 POP3 密码形式下用户root的密码写入root1234（见图8覆盖处，请按标准填写）

【正确答案】：root1234

【填空题】使用 Bruter 基于密码字典破解MSSQL密码结果写入123456（见图10覆盖处，请按标准填写）

【正确答案】：123456

【填空题】使用 Bruter 基于密码字典破解HTTP密码的结果写入123456（见图17覆盖处，请按标准填写）

【正确答案】：123456

ABAAB

{% endfolding %}

{% folding child:codeblock open:false 网络服务远程密码破解（Hydra）实验 %}

【填空题】请将图2覆盖处使用 hydra 工具基于密码字典破解结果写出来1q2w3e4r

【正确答案】：1q2w3e4r

【填空题】请将图3覆盖处基于密码字典破解结果写出来123456

【正确答案】：123456

【填空题】请将图4覆盖处使用 hydra 工具基于字典破解结果写出来123456

【正确答案】：123456

【填空题】请将图7覆盖处使用 hydra 工具基于密码字典破解结果写出来123456

【正确答案】：123456

ABCB

{% endfolding %}

{% folding child:codeblock open:false 口令破解-01HASH基础实验 %}

【填空题】请将使用HashCale工具进行文件加密计算后的MD5值写出efd（见图3覆盖处，请按标准填写）



【正确答案】：efd

【填空题】请将使用WinMD5工具校验出的MD5值写出4532（见图5覆盖处，请按标准填写）



【正确答案】：4532

【填空题】请将加密后的MD5值写出7a57a5a743894a0e（见图7覆盖处，请按标准填写）



【正确答案】：7a57a5a743894a0e

【填空题】请将从网页上获得的MD5值写出499d（见图13覆盖处，请按标准填写）



【正确答案】：499d

CBA

{% endfolding %}

{% folding child:codeblock open:false 口令破解MD5实验 %}

【填空题】请将“love”的MD5加密后的值填写出来 fe309af0f4d35982（答案见图3遮盖处，请标准填写）



【正确答案】：fe309af0f4d35982

DDC

{% endfolding %}

{% folding child:codeblock open:false access口令破解实验 %}

【填空题】请将使用access数据库操作口令破解结果写出来123456（见图3覆盖处，请按标准填写）



【正确答案】：123456

ACBAD

{% endfolding %}

{% folding child:codeblock open:false Office密码破解实验 %}

【填空题】请将破解出来的十六进制格式密码写出来3600（见图10覆盖处，请按标准填写）



【正确答案】：3600

{% endfolding %}

{% folding child:codeblock open:false wifi密码破解实验 %}

滑下去点下一实验就行

{% endfolding %}

{% folding child:codeblock open:false FTP远程密码破解实验 %}

【填空题】在TCP/IP协议中，FTP标准命令TCP端口号为21，Port方式数据端口为20（答案见实验原理，请按标准阿拉伯数字填写）



【正确答案】：20

【填空题】在实验中，FTP破解工具通过数据端口和字典破解的结果为123456（答案如图11遮盖处，请按标准填写）



【正确答案】：123456

ADCBA

{% endfolding %}

{% folding child:codeblock open:false 压缩文件解密实验 %}

【填空题】请将破解出来的16进制密码结果写出来（6位阿拉伯数字）313233（见图8覆盖处，请按标准填写）



【正确答案】：313233

CBA

{% endfolding %}

### SQL注入漏洞攻击

#### SQL注入初探

{% folding child:codeblock open:false ASPX的SQL基础注入攻击实验 %}


【填空题】Pangolin程序查看到SQL注入漏洞目标机的数据库名称为master（答案详细见图9覆盖内容）



【正确答案】：master


【填空题】Pangolin自定义查询username like 'admin%'查询到admin用户的密码为admin123（答案详细见图13覆盖内容）



【正确答案】：admin123


【填空题】Pangolin 的Dir Tree功能查看到数据库超级管理员sa的密码为123456（答案详细见图19覆盖内容）



【正确答案】：123456

BDDDA

{% endfolding %}

{% folding child:codeblock open:false jsp的mysql注入攻击实验 %}

??

{% endfolding %}

{% folding child:codeblock open:false PHP的SQL基础注入攻击实验 %}


【填空题】Pangolin程序查看到SQL注入漏洞目标机的数据库名称为wordpress（答案详细见图9覆盖内容）



【正确答案】：wordpress


【填空题】Pangolin自定义查询user_login like CHAR(37, 97, 100, 109, 105, 110, 37)查询到admin用户的email账号为admin@example.org（答案详细见图14覆盖内容）



【正确答案】：admin@example.org


【填空题】Pangolin查看用户的基本属性，sys用户的主目录为/dev（答案详细见图15覆盖内容）



【正确答案】：/dev

DBDDA

{% endfolding %}

{% folding child:codeblock open:false Mutillidae登录认证绕过实验 %}


【填空题】该实验利用如上方法进行sql注入绕过认证登录的用户名称为admin（答案详细见图8覆盖内容）



【正确答案】：admin

【填空题】11



【正确答案】：1

【填空题】11



【正确答案】：1

3【填空题】11



【正确答案】：1

4【填空题】11



【正确答案】：1

5【填空题】11



【正确答案】：1

{% endfolding %}

{% folding child:codeblock open:false Mutillidae读取文件内容实验 %}


【填空题】file出错信息中查看出错文件的路径为/owaspbwa/mutillidae-git/classes/MySQLHandler.php（答案详细见图3覆盖内容,注意大小写）



【正确答案】：MySQLHandler.php

ADDDC

{% endfolding %}

{% folding child:codeblock open:false Mutillidae获取数据库内容实验 %}



【填空题】该实验利用如上方法查询到当前数据库中“accounts”表的第三条数据列名为password（答案详细见图8覆盖内容）



【正确答案】：password

DDDDC

{% endfolding %}

{% folding child:codeblock open:false POST方式SQL注入攻击实验 %}


【填空题】sqlmap扫描wackopicko 库中 users 表的第9个用户是wanda（答案详细见图24覆盖内容）



【正确答案】：wanda

【填空题】sqlmap扫描wackopicko 库中 admin 表的第5个用户是bob（答案详细见图27覆盖内容）



【正确答案】：bob

ADADC

{% endfolding %}

{% folding child:codeblock open:false GET方式SQL注入攻击实验 %}


【填空题】sql注入报错法获取到登录的用户名为admin（答案详细见图12覆盖内容）



【正确答案】：admin


【填空题】通过绕过waf过滤措施注入获取到admin用户的邮箱为admin@example.org（答案详细见图16覆盖内容）



【正确答案】：admin@example.org


【填空题】sqlmap扫描到该实验目标机的PHP版本为5.5.9（答案详细见图24覆盖内容）



【正确答案】：5.5.9


【填空题】利用sqlmap的tamper脚本获取wordpress库中关于wp_users表的第一个用户名为admin（答案详细见图41覆盖内容）



【正确答案】：admin

ADADC

{% endfolding %}

{% folding child:codeblock open:false SQL注入漏洞攻击实验 %}


【填空题】TamperData查看到Cache-Control取值为private（答案详细见图9覆盖内容）



【正确答案】：private


【填空题】sqlmap扫描到该实验目标机的iis版本为6.0（答案详细见图17覆盖内容）



【正确答案】：6.0


【填空题】字典猜解获取tb_admin表的admin用户密码为1b7f1c73a481e240（答案详细见图24覆盖内容）



【正确答案】：1b7f1c73a481e240

ADADC

{% endfolding %}

{% folding child:codeblock open:false 宽字符绕过转义防护的SQL注入攻击实验 %}

??

{% endfolding %}

#### 手工SQL注入

{% folding child:codeblock open:false 手工注入之MySQL注入基础实验 %}


【填空题】页面出错信息中查看警告文件的路径为/var/www/html/zvuldrill/search.php（答案详细见图4覆盖内容,注意大小写）



【正确答案】：search.php


【填空题】本实验查询到admin的第三个列标题的内容是abc（答案详细见图5覆盖内容）



【正确答案】：abc

ADDDC

{% endfolding %}

{% folding child:codeblock open:false 手工注入之MySQL手工布尔型注入实验 %}


【填空题】成功判断出数据库列名后，显示的第二条留言内容为1234（答案详细见图7覆盖内容）



【正确答案】：1234


【填空题】爆库得到admin用户的密码为c4da997（答案详细见图15覆盖内容）



【正确答案】：c4da997

DADDC

{% endfolding %}

{% folding child:codeblock open:false 手工注入之MySQL手工时间型注入实验 %}


【填空题】访问的网页的类型是html（答案详细见图4覆盖内容）



【正确答案】：html


【填空题】时间型注入得到第一行的数据库的名称为dvwa（综合2.8-2.12操作得出或将ascii翻译成所表示的字符）



【正确答案】：dvwa

DADDC

{% endfolding %}

{% folding child:codeblock open:false 手工注入之MySQL文件读取实验 %}


【填空题】读取到后台的密码的hash值最后5位值是da997（答案详细见图9覆盖内容）



【正确答案】：da997

DDDDC

{% endfolding %}

{% folding child:codeblock open:false 手工注入之MySQL手工注入写一句话shell %}


【填空题】爆出的网页目录的绝对路径为/var/www/html/zvuldrill（答案详细见图3覆盖内容,注意大小写区分）



【正确答案】：/var/www/html/zvuldrill


【填空题】利用union select..into outfile语句将查询到的内容及一句话木马写入文件,union查询到关于“1”字符的留言第二条的内容为1234（答案详细见图5覆盖内容）



【正确答案】：1234


【填空题】查看到search.php最后一句内容，把footer.php包含进现在的文件里来（答案详细见图12覆盖内容）



【正确答案】：footer.php

DADDC

{% endfolding %}

{% folding child:codeblock open:false 手工注入之MySQL手工字符型注入实验 %}


【填空题】成功判断出数据库列名后，显示的第二条留言内容为1234（答案详细见图7覆盖内容）



【正确答案】：1234


【填空题】爆库得到admin用户的密码最后5位为da997（答案详细见图13覆盖内容）



【正确答案】：da997

DADCC

{% endfolding %}

{% folding child:codeblock open:false 手工注入之MySQL手工宽字节注入实验 %}

??

{% endfolding %}

{% folding child:codeblock open:false 手工注入之post手工注入实验 %}

DADAC

{% endfolding %}

{% folding child:codeblock open:false 手工注入之cookie手工注入实验 %}


【填空题】实验所用的 SQLMap 的版本号为：1.0（见图5覆盖处，请按标准填写）



【正确答案】：1.0


【填空题】利用 SQLMap 扫描得到的数据表信息中，被遮挡的数据表为：news（见图8覆盖处，请按标准填写）



【正确答案】：news

【填空题】利用 SQLMap 扫描得到的数据表信息中，被遮挡的数据表为：news（见图9覆盖处，请按标准填写）



【正确答案】：news


【填空题】利用 SQLMap 扫描得到的字段信息中，被遮挡的字段为：id（见图10覆盖处，请按标准填写）



【正确答案】：id

【填空题】利用 SQLMap 扫描得到的字段信息中，被遮挡的字段为：id（见图12覆盖处，请按标准填写）



【正确答案】：id


【填空题】利用 SQLMap 扫描得到的用户信息中，被遮挡的用户密码为：admin（见图12覆盖处，请按标准填写）



【正确答案】：admin

【填空题】利用 SQLMap 扫描得到的用户信息中，被遮挡的用户密码为：admin（见图14覆盖处，请按标准填写）



【正确答案】：admin

DBCAD BBCBA

{% endfolding %}

#### SQL注入深入

{% folding child:codeblock open:false sql注入--基于错误 %}


【填空题】一般判断是否存在基于错误的盲注和显错注入，可以输入【　　】，有报错信息，说明存在注入。（直接填写英文符号，填写中文名称不得分）
'



【正确答案】：'


【填空题】从报错信息 ''1'') 可以看出$id参数被【　　】包裹着。（答案见步骤4.1，按标准格式填写）
('')



【正确答案】：('')

ADAB

{% endfolding %}

{% folding child:codeblock open:false 宽字节注入 %}


【填空题】sqlmap的哪个参数可以读取服务端任意文件（请按标准格式填写，注意符号）--file-read



【正确答案】：--file-read

ADABB

{% endfolding %}

{% folding child:codeblock open:false sql盲注--基于布尔 %}


【单选题】sqlmap注入方式technique，基于Boolean的盲注的参数是

A. Q

B. B

C. T

D. U

【正确答案】：B

ABBB

{% endfolding %}

{% folding child:codeblock open:false sql盲注--基于报错 %}


【填空题】哪个数据库可以使用`exp(~(select * from(select database())as a ))`查询到数据库名（填写“mariadb”或“mysql”）
mysql



【正确答案】：mysql


【单选题】本次实验中，管理员密码使用的加密是：

A. AES

B. SHA1

C. MD5

D. ECC

【正确答案】：C

ADAB

{% endfolding %}

{% folding child:codeblock open:false sql盲注--基于时间 %}

【填空题】sleep(5)表示延时5【　　】（填写时\分\秒\毫秒，不要填写英文字符）
秒

【正确答案】：秒

DBA

{% endfolding %}

{% folding child:codeblock open:false sql注入导入导出 %}


【单选题】网址`http://192.168.15.86/phpaa/search.php?keywords=1' union select 1,2,3,4,5,6,7,8,0x3c3f70687020406576616c28245f504f53545b6872736166655d293b3f3e,9,10,12,13,14 into outfile '/var/www/html/yjh.php' -- '`中，一句话木马是以多少进制的形式存在的

A. 2

B. 8

C. 10

D. 16

【正确答案】：D

BACBB DD

{% endfolding %}

{% folding child:codeblock open:false 增删改函数使用及注入防御方法 %}


【填空题】哪个函数指定了转义字符（答案见原理，按标准格式填写，只填写函数名即可）addslashes()



【正确答案】：addslashes()

BCACC

{% endfolding %}

{% folding child:codeblock open:false http头部注入 %}


【单选题】sleep(5)的时间单位是

A. ms

B. s

C. m

D. h

【正确答案】：B


【填空题】burpsuit中的【】模块可以进行编解码（使用小写英文字符）decoder



【正确答案】：decoder


【填空题】sqlmap的哪个选项表示从文件读取数据（按标准格式填写）-r



【正确答案】：-r

DCDBB

{% endfolding %}

{% folding child:codeblock open:false 堆叠注入 %}


【填空题】若在步骤2.3，想查看数据库名称，可以把 version() 换为【　　】（使用小写英文字符）
database()



【正确答案】：database()


【填空题】sqlmap中的哪个选项可以导入文本文件的数据（使用英文符号和字母）
-r



【正确答案】：-r

BABC

{% endfolding %}

{% folding child:codeblock open:false sqlmap工具使用 %}


【填空题】哪个选项可以指定字段（按标准格式填写，注意符号）
-c



【正确答案】：-c

AABCA

{% endfolding %}

{% folding child:codeblock open:false 二次注入 %}

【单选题】当注册用户时存在用户名字符数限制时，可以使用的工具是？

A. Vega

B. BurpSuite

C. Nmap

D. SQLmap

【正确答案】：B

BACAC

{% endfolding %}

{% folding child:codeblock open:false sqlmap深入 %}


【填空题】获取shell权限使用的sqlmap参数命令为（请使用标准格式填写）
--os-shell



【正确答案】：--os-shell

BABBC

{% endfolding %}

### CSRF跨站请求伪造攻击

{% folding child:codeblock open:false 利用burp生成POC %}

答案全是1....

{% endfolding %}

{% folding child:codeblock open:false CSRF实战cms %}

答案还是1....

{% endfolding %}

### Web密码破解攻击

{% folding child:codeblock open:false 登录表单密码破解攻击（Mutillidae）实验 %}

【填空题】使用Burp对登录信息进行拦截时，其中数据包格式中login-php-submit-button=____（见图16覆盖处，请按标准填写）

【正确答案】：Login

DDCC

{% endfolding %}

{% folding child:codeblock open:false 登录表单密码破解攻击（wzaspshop）实验 %}

【填空题】使用burp对登录信息进行拦截时，其中数据包格式中动作action=____（见图11覆盖处，请按标准填写）

【正确答案】：login

【填空题】破解结果中， 可以看到密码为qwerasdf的状态返回长度Length是____（见图20覆盖处，请按标准填写）

【正确答案】：356

CDCD

{% endfolding %}

## 实验4{% emoji blobcat ablobcatwave %}

### 日志清除

#### Linux系统日志清除

{% folding child:codeblock open:false linux系统日志清除实验 %}

【填空题】在Linux系统中，使用lastlog命令可以查询每个用户最后一次登录的设备号和时间。（答案参考2.3）

【正确答案】：lastlog

【填空题】logtamper后面可以跟三种参数，它们分别是 -h、-m 和 -w

【正确答案】：-w

【填空题】logtamper后面跟-m参数可以修改用户最后一次登录日志

【正确答案】：-m

ABD

{% endfolding %}

{% folding child:codeblock open:false linux系统清除日志 %}

DDD

{% endfolding %}

{% folding child:codeblock open:false Linux中清除痕迹和隐藏自己 %}

DDDBC

{% endfolding %}

#### Windows系统日志清除

{% folding child:codeblock open:false WindowsXP系统日志清除实验 %}

【填空题】使用elsave -l security -C命令删除所有安全日志，并新添加了一条日志，它的分类是系统事件。（见图30遮盖处，注意事件为517）

【正确答案】：系统事件

ABCD

{% endfolding %}

{% folding child:codeblock open:false Windows 7系统日志清除实验 %}

【填空题】在事件查看器中，Windows日志中主要包含“应用程序”、“安全”、“Setup” 、系统以及“转发事件”。 （答案见图9覆盖处，请按标准填写）

【正确答案】：系统

【填空题】在Windows中，使用wevtutil.exe cl “Security”命令可以清除安全日志。（答案参考图11，请标准填写）

【正确答案】：Security

DCB

{% endfolding %}

{% folding child:codeblock open:false Windows2003系统日志清除实验 %}

【填空题】在本实验中，清除Windows日志使用了del \*.\*命令。 （答案见图18处，请标准填写）

【正确答案】：del \*.\*

ACD

{% endfolding %}

{% folding child:codeblock open:false Windows2008系统日志清除实验 %}

【填空题】在Apache日志的语句中，带有“logCheck”进项暴力破解的路径，其请求方式为POST。（见图8覆盖处，请按标准填写）

【正确答案】：POST

CBA

{% endfolding %}

