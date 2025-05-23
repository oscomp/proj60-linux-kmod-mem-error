# proj60-linux-kmod-mem-error

### 项目描述

Linux 内核支持动态加载模块，这大大提高了程序开发的灵活性，使得众多驱动可以独立开发和加载运行。但是 Linux 是宏内核，内核模块如果出现访存错误，仍然会导致系统crash。包括：

* 内核模块越界访问修改内存内容，导致其他模块，或系统crash。
* 内核模块访问空指针，导致系统 crash。
* 内核模块随机访问其他系统地址，导致系统crash。

内存访存错误是系统中常见的错误，内核中无论是核心模块还是众多驱动，只要出现访存错误，都会引起系统异常或崩溃。因此将驱动模块的错误隔离在驱动本身，而不影响系统和其他模块，非常有意义。

### 所属赛道

2025全国大学生操作系统比赛的“内核实现”赛道



### 参赛要求

- 以小组为单位参赛，最多三人一个小组，且小组成员是来自同一所高校的本科生=
- 如学生参加了多个项目，参赛学生选择一个自己参加的项目参与评奖
- 请遵循“2025全国大学生操作系统比赛”的章程和技术方案要求



### 项目导师

谢秀奇

* gitee [Xie XiuQi](https://gitee.com/xiexiuqi)

* email xiexiuqi@huawei.com



### 难度

困难



### 特征

- 实现严重内核模块内存的管理方式，模块内如果出现访存错误，不影响其他模块，和系统
- 模块访存性能不出现明显的下降

### 文档

[Linux物理内存页面分配](http://ilinuxkernel.com/?p=1371)

### License

- GPLv2 (https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)

## 预期目标

### 注意：下面的内容是建议内容，不要求必须全部完成。选择本项目的同学也可与导师联系，提出自己的新想法，如导师认可，可加入预期目标



### 基于 Linux kernel 4.19 或 5.10 或社区主线实现

* 完成相关内核代码，可以编译安装运行
* 构造内核模块（ko），模拟测试
* 模块中存在内存访问错误，系统报错，不影响系统其他模块和子系统运行。
* 补丁发送到社区主线（可选）

