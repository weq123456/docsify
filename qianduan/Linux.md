#                                             Linux

## 根目录的介绍

>/bin 二进制可执行命令
>
>/dev 设备特殊文件
>/etc 系统管理和配置文件
>/etc/rc.d 启动的配置文件和脚本
>/home 用户主目录的基点，比如用户user的主目录就是/home/user，可以用~user表示
>/lib 标准程序设计库，又叫动态链接共享库，作用类似windows里的.dll文件
>/sbin 超级管理命令，这里存放的是系统管理员使用的管理程序
>/tmp 公共的临时文件存储点
>/root 系统管理员的主目录
>/mnt 系统提供这个目录是让用户临时挂载其他的文件系统
>/lost+found这个目录平时是空的，系统非正常关机而留下“无家可归”的文件（windows下叫什么.chk）就在这里
>/proc 虚拟的目录，是系统内存的映射。可直接访问这个目录来获取系统信息。
>/var 某些大文件的溢出区，比方说各种服务的日志文件
>/usr 最庞大的目录，要用到的应用程序和文件几乎都在这个目录，其中包含：
>
>/usr/x11R6 存放x window的目录
>/usr/bin 众多的应用程序
>/usr/sbin 超级用户的一些管理程序
>/usr/doc linux文档
>/usr/include linux下开发和编译应用程序所需要的头文件
>/usr/lib 常用的动态链接库和软件包的配置文件
>/usr/man 帮助文档
>/usr/src 源代码，linux内核的源代码就放在/usr/src/linux里
>/usr/local/bin 本地增加的命令
>/usr/local/lib 本地增加的库根文件系统

## 常用的命令

> ls  列出目录
>
> ls -a 查看所有的文件，包括隐藏文件
>
> ls -l  列出文件信息
>
> ls -al 列出隐藏文件信息
>
> mkdir test  创建文件目录
>
> mkdir  -p test1/tets2/test3 创建多级目录
>
> pwd  显示当前用户目录
>
> rmdir test 删除文件
>
> rmdir -p  test1/test2 删除多级文件
>
> cp  install.sh  haitian  复制文件
>
> rm -rf  install.sh  删除文件  
>
> -f–是忽略不存在的文件，不会出现警告，强制删除
>
> -r递归删除文件
>
> -i 互动，删除询问是否删除
>
> mv  install.sh  test 移动文件/重命名文件
>
> ifconfig  查询网络配置
>
> tav  -zxvf xxxx解压文件

## 文件内容查看

> cat  由第一行开始显示文件内容，用来读文章或者读取配置文件，都使用cat名
>
> cat instatll.sh
>
> nl cat install.sh
>
> tac  从最后一行开始显示，可以看出tac是cat的倒着写
>
> nl 显示的时候，顺便输出行号
>
> more  一页一页的显示文件内容
>
> less 与 more类似，但是比more更好的是，他可以往前翻页
>
> q退出 /查询字符串，n向下一个，N向上一个
>
> head 只看头几行
>
> tail 只看尾巴几行

## Linux链接

> Linux 连接分两种： 硬链接，软连接
>
> 硬链接：A--B,假设B是A的链接，那么他们俩个指向了同一个文件，允许一个文件拥有多个路径，用户可以通过这种机制建立硬链接到一些重要文件上，防止误删。
>
> 软链接：类似window下的快捷方式，删除的源文件，快捷方式也访问不饿了
>
> 创建链接  ln命令
>
> 创建软连接  ln -s f1 f3
>
> touch  命创建文件
>
> echo 输入字符串
>
> echo “I love you” >> f1

## Vim编辑器

> 常用的命令
>
> i 切换道输入模式，以输入字符
>
> x删除当前光标所在的字符。
>
> ：切换到底线命令模式，以在最低一行输入命令
>
> EXC退出编辑模式返回命令模式
>
> :q ！强制退出
>
> :wq 保存退出
>
> ：set nu行号
>
> ： set nonu 取消行号
>
> /sdfa  搜索
>
> 

## 文件属性

常用的命令

> 1，chgrp: 更改文件属性
>
> chgrp -R 属组名 文件名
>
> 2，chown: 更改文件属性，也可以同时更改 文件属组
>
> chown -R 属组名 文件名
>
> chown  -R  属主名:属组名  文件名
>
> 3，chmod: 更改文件9个属性
>
> chmod  -R   xyz （文件或目录）
>
> Linux文件属性有两种设置方法，一种是数字，一种是符号
>
> Linux文件的基本权限就有九个，分别是owner/group/others三种身份各有自己的read/write/execute权限
>
> 文件的权限字符为：【-rwxrwxrwx】,这九个权限是三个三个一组的，其中，我们可以使用数字来代表各个权限，各权限的分数对照表如下：
>
> r:4  w:2  x:1
>
> 可读可写不可执行  rw-      2+4 =6
>
> 可读可写可执行    rwx      2+4+1 =7
>
> chomd 777  text.txt文件属于所有用户可读可写可执行
>
> 

## Linux账号管理

> useradd -m haitian   添加用户
>
> -m: 自动创建这个用户的主目录 /home/haitian
>
> -G :给用户分配用户组
>
> cat /etc/passwd  查看用户信息
>
> userdel  -r haitian  删除用户
>
> usermod -d  /home/233/ haitian  修改用户 查看配置文件 cat/etc/passwd
>
> su  haitain  切换用户  exit 退出用户
>
> hostname  主机名    hostname   haitian   修改
>
> passwd  haitian  修改用户密码
>
> passwd -1 haitian  冻结账号
>
> passwd -d haitian    清除密码 不能再登录
>
> 密码真正存放的密码 放在  /etc/shadow
>
> 

## 用户组管理

属主  属组

> 每个用户都有一个用户组，系统可以对一个用户组中的所有用户进行集中管理。不同Linux系统对用户组的规定有所不同，如Linux下的用户属于与它同名的用户组，这个用户组在创建用户时同时创建。组的添加，删除，修改，都是对 /etc/group/文件的更新。

> 创建用户组
>
> groupadd test  
>
> -g 520 指定id号
>
> cat /etc/group 查看用户组信息
>
> groupdel www 删除用户组
>
> groupmod -g 666 -n  test1  test  修改用户组
>
> newgrop root

## 磁盘管理

> df -h    查看磁盘使用情况
>
> du -sm /*   查看根目录下每个目录所占用的容量
>
> Mac 或者想使用Linux挂载我们的一些本地磁盘或者文件
>
> mount  /dev/haitian  /mnt/haitian  
>
> dev 下面是外部设备haitian，/mnt/挂载到mnt目录下，来实现访问  
>
> umount -f  强制卸载

## 进程管理

> ps 查看当前系统中正在执行的各种进程的信息
>
> ps -xx:
>
> ​    -a 显示当前终端运行的所有的进程信息（当前的进程一个）
>
> ​     -u  以用户的信息显示进程
>
> ​      -x   显示后台运行进程的参数
>
> ps -aux  查看所有的进程
>
> ps  -aux |grep   xxx   查看某功能的进程，如java，MySQL
>
> | 这个在Linux中叫做管道符
>
> grep  过滤，查找文件中符合条件的字符串
>
> ps -ef |grep   xxx 查看父进程
>
> pstree -pu   进程树
>
> ​    -p   显示父id
>
> ​     -u   显示用户组
>
> kill  -9   进程号   杀死进程

## 环境安装

> 安装软件一般有三种方式： rpm,解压缩，yum在线安装
>
>  /etc/profile  配置环境变量
>
> 让配置生效  source   /etc/profile
>
> firewall-cmd --list-ports  查看防火墙开的端口
>
> firewall-cmd --zone=public --add-port=9000/tcp --permanent   防火墙开启端口
>
> systemctl restart  firewalld.service   防火墙重启

### JDK安装

> vim   /etc/profile





