# 项目描述
  * 跟着郑刚老师的《操作系统真象还原》做的简易操作系统练习项目（强烈推荐这本书）
    ![cover](./images/cover.jpg)

#### 运行环境
  * bochs2.6.2
  * CentOS 6.3
  * 我是按照书上的原环境，换 ubuntu 或 bochs 最新版本 之类的也行，自行修改下配置就行

#### 编译&运行
  * 添加 bochs/bin 到环境变量中，之后 make all 即可
  * 可以运行 run.sh 来检测环境并运行，也可以自行 bochs -f your_bochs_configure_file

#### 代码架构说明
``` 
|-- 根目录
    |-- src 主要的开发目录
    | |-- boot/                开机初始化文件
    | |-- command/             OS 可执行的命令（可自行添加）
    | |-- device/              外设相关（接口中断、管道等）
    | |-- fs/                  文件相关
    | |-- kernel/              内核
    | |-- lib/                 库文件
    | |-- shell/               shell（我们与系统交互的接口）
    | |-- thread/              进程线程相关
    | |-- userprog/            用户内核
    | |-- bochsrc.disk         bochs 配置文件
    | |-- makefile             make 源码编译
    | |-- run.sh               快速运行脚本
```

如果有问题，请提 issue 说明 => [传送门](https://github.com/Yanzu-zz/OS-Simplicity)
