# 一、SHELL技术
1. SHELL 特性
2. SHELL 变量
3. SHELL 条件测试
4. SHELL 数值运算
5. 流程控制,循环
```shell
    if
    case
    for
    while
    until
    break
    continue
    exit
    shift
    array
    function
```
6. 企业项目

# 二、shell? 命令解释器
shell 命令



系统级             登录的时候会执行

/etc/profile         /etc/profile

                     ~/.bash_profile

                     ~/.bashrc         

/etc/bashrc          /etc/bashrc  

用户级

~/.bash_profile    离开shell会执行

~/.bashrc           /etc/bashrc  

~/.bash_history     ~/.bashrc 

~/.bash_logout

# 三、GUN/bash shell特点
1. 命令和文件自动补齐
2. 命令历史记忆功能 上下键。!number,!string,!$,!!,^R
3. 别名狗功能 alias,unalias cp,~username/.bashrc,\cp -rf /etc/hosts
4. 快捷键 ^R,^D,^A,^E,^L,^U,^K,^S,^Q
5. 前台，后台作业控制 &、nohup、^C、^Z、bg%1、fg%1、kill %3、screen
6. 输入输出重定向0,1,2 >  >>  2> 2>>  2>&1 &1>  cat < /etc/hosts cat <<EOF  
cat >file1 <<EOF
    
    [root@zhangzeli-node1 ~]# ll /dev/std\*

    lrwxrwxrwx. 1 root root 15 4月  23 10:52 /dev/stderr -> /proc/self/fd/2

    lrwxrwxrwx. 1 root root 15 4月  23 10:52 /dev/stdin -> /proc/self/fd/0

    lrwxrwxrwx. 1 root root 15 4月  23 10:52 /dev/stdout -> /proc/self/fd/1

7. 管道 | tee
    
    ip addr |grep 'inet' |grep eth0

    [root@zhangzeli-node1 scripts]# date >date.txt

    [root@zhangzeli-node1 scripts]# date |tee date.txt 
    
    2019年 04月 23日 星期二 16:44:12 CST
8. 命令排序
    
    ; 不具备逻辑判断

    && || 具备逻辑判读

    ./configure && make && make install (命令返回值 echo $?)

    注意：

    command &             后台执行

    command &> /dev/null  混合重定向(标准输出1，错误输出2)

    command1 && command2 命令排序，逻辑判断
9. shell的通配符(元字符)
    
    \* 匹配任意多个字符

    ? 匹配任意一个字符 touch love loove live  l7vel;||ll l?ve

    [] 匹配括号中的任意**一个**字符[abc] [a-z] [0-9] [a-zA-Z0-9]

    () 在子shell中执行(cd /boot;ls) (umask 077;touch file1000)

    {}集合 touch file{1..9}

10. 变量

11. 脚本
