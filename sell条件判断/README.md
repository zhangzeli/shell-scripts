```shell
read -p "Please input number：" num

while true
do
    if [[ "$num" =~ ^[0-9]+& ]];then
        break
    else
        read -p "不是数字，请重新输入数值： " num
    fi
done
```
### 符号

>() 子shell  

>(()) 数值比较，运算，C语言  

>$() 命令替换  

>$(()) 整数运算  

>{} 集合  

>${}  

>[] 条件测试  

>[[]] 条件测试 支持正则 =~  

>$[] 整数运算  

### 执行脚本

>./  01.sh        **需要执行权限** 在子shell 中执行  
>bash 01.sh        不需要执行权限   在子shell 中执行  
>. 01.sh          不需要执行权限   在当前shell中执行
>source            不需要执行权限  在当前shell中执行
tip:通常修改系统配置文件如 /etc/profile 的path等变量后，使之在当前shell中生效

### 调试脚本
>sh -n  仅调试syntax error  
>sh -vx  以调试的方式执行，查询整个执行过程  
