# Linux Self-learnng 
## 20220918 
- Grep
鸟哥的linux私房菜 - regular expression
>“语法： [root @test /root ]# grep [-acinv] '搜寻字符串' filename

>参数说明：

>-a ：将 binary 档案以 text 档案的方式搜寻数据

>-c ：计算找到 '搜寻字符串' 的次数

>-i ：忽略大小写的不同，所以大小写视为相同

>-n ：顺便输出行号

>-v ：反向选择，亦即显示出没有 '搜寻字符串' 内容的那一行！

>范例：

```
[root @test /root]# grep 'root' /var/log/secure # 将 /var/log/secure 这个档案中有 root 的那一行秀出来

[root @test /root]# grep -v 'root' /var/log/secure # 若该行没有 root 才将数据秀出来到屏幕上！

[root @test /root]# last | grep root # 若该行有 root 才将数据秀出来到屏幕上！

[root @test /root]# grep [A-Z]ANPATH /etc/man.config # 将 /etc/man.config 这个档案当中，所有有：

```
