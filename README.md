# PA_selflearning



# Day1

PA0完成

- [x] installing GNU/Linux
- [x] Learn more about VIM, GDB, tmux



GDB using 

```shell
gcc -g test.cpp
lldb a.out
```

![image-20200802215849193](img/image-20200802215849193.png)

![image-20200802215945672](img/image-20200802215945672.png)

![image-20200802220019900](img/image-20200802220019900.png)

<img src="img/image-20200804130827095.png" alt="image-20200804130827095" style="zoom:80%;" />

<img src="img/image-20200804131040174.png" alt="image-20200804131040174" style="zoom:80%;" />



<img src="img/image-20200804132041557.png" alt="image-20200804132041557" style="zoom:80%;" />



makefile中PHONY的作用

Tmux入门: https://linux.cn/article-3952-1.html





Some problems:

* 在将username加到sudo的时候

```shell
su -   # we still need to switch to the root account first
adduser username sudo  # change `username` to your user name
```

bash: adduser: command not found

解决方法: 

Adding `sbin` to path seems to at least temporarily fix the problem for me:

```
export PATH="$PATH:/sbin:/usr/sbin:usr/local/sbin"
```

Or try executing 

```
/sbin/useradd
```

> 惊了，将username加到了sudo后不知道怎么就一直不能通过sudo访问，重启了之后就好了，估计重启了之后才能起作用



# Day3

https://www.cnblogs.com/qingergege/p/5914218.html

```cpp
getopt()
```

选项字符串："a: b:cd::e"，由getopt(argc, argv, "ab:c: de::")函数的第三个参数指定。
	
选项：分带参和不带参选项 ，执行命令时，选项可有可无，如-b,-c等等。选项后的冒号表示参数，一个冒号就表示这个选项后面必须带有参数，不带参数报错。



```cpp
char *strtok(char *str, const char *delim)
```

https://www.runoob.com/cprogramming/c-function-strtok.html

当strtok()在参数s的字符串中发现参数delim中包含的分割字符时,则会将该字符改为\0 字符。在第一次调用时，strtok()必需给予参数s字符串，往后的调用则将参数s设置成NULL。每次调用成功则返回指向被分割出片段的指针。





```cpp
parse_args;
init_log;
load_img; 将客户程序从镜像文件读入到客户计算机的内存;
init_isa;

```



If you press Ctrl + w, followed by Shift + n, it pauses the terminal, and you can navigate it like any buffer. Pressing i takes you back into the terminal as you were before.

















