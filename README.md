# Shell 运用
1. 自动化批量系统初始化(update,软件安装，时区设置，安全策略...)
2. 自动化批量软件部署程序(LAMP,LNMP,Tomcat,LVS,Nginx)
3. 管理应用程序(KVM,集群管理扩容，MySQL)
4. 日志分析处理程序(PV,UV,200,!200,TOP100,grep/awk)
5. 自动化备份恢复程序(MySQL完全备份/增量+Crond)
6. 自动化管理程序(批量远程修改密码,软件升级，配置更新)
7. 自动化信息采集以及监控程序(手机系统/应用状态信息,CPU,Mem,Disk,Net,TCP Status,Apache,MySql)
8. 配合Zabbix信息采集(手机系统/应用状态信息,CPU,Mem,Disk,Net,TCP Status,Apache,MySql)
9. 自动化扩容(增加云主机 ----> 业务上线)
    zabbix监控CPU(80%+|-50%) + Python API AWS/EC2(增加/删除云主机)+Shell +Script(业务上线)
10. 俄罗斯方块，打印三角形，打印圣诞树，打印五角星，运行小火车，坦克大战,排序算法(能力有限)

## 程序语言执行:
```
C       ---- 编译 ------ 二进制机器码 (CPU X86复杂指令集，Power精简指令集，APM)

Java    ---- 编译-------字节码(Java虚拟机 JDK) Tomcat/Hadoop

Shell   ---- 解释 (/usr/bin/bash)
perl    ---- 解释 (/usr/bin/perl)
expect  ---- 解释 (/usr/bin/expect)

Python  ---- 解释 (/usr/bin/python)
        ---- 编译 ----- 字节码(Python虚拟机)

程序是由那些组成的: 逻辑+数据
```
