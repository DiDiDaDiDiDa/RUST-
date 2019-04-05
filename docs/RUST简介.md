

# RUST简介

Rust 是 Mozilla 开发的注重安全、性能和并发性的编程语言。Rust 是针对多核体系提出的语言，并且吸收一些其他动态语言的重要特性，比如不需要管理内存，比如不会出现 Null 指针等。

### 适用人群：

​	因为里面有很多泛型，可能比较适用于C和C++的开发者，由于我只写过Java和GO所以得好好努力了！

### 基本介绍：

rust是一门强调安全、性能和并发性的系统编程语言。为了达到此目的，甚至没有垃圾回收器，同时这样做也使得Rust能够应用到其他语言做不到的地方：嵌入到其他语言，有指定空间和时间需求的程序，写底层代码（如设备驱动程序和操作系统）。针对当前的其他编程语言，Rust 做到了没有运行时(Runtime)，没有数据竞争。 Rust 也致力于实现“零成本抽象”，尽管这些抽象给人的感觉像一个高级的语言。即使是这样，Rust 仍然可以做到像一个低级的语言那样的精确控制。

### 安装

我用的mac，所以只有mac的。

1，打开terminal

```
$ curl -sf -L https://static.rust-lang.org/rustup.sh | sh
```



![image-20190403141703029](https://github.com/DiDiDaDiDiDa/RUST-/blob/master/docs/images/image-20190403141703029.png)

输入 1  即默认安装。如果输入2 自定义安装。输入3，取消安装，这里我们输入1.

###### 当然！我在下载的过程中碰到这个问题！

![image-20190403143310409](https://github.com/DiDiDaDiDiDa/RUST-/blob/master/docs/images/image-20190403143310409.png)

解决办法， 

```
# 编辑文件
$ vim ~/.bash_profile
# 在文件中加入以下两句
export RUSTUP_DIST_SERVER=https://mirrors.ustc.edu.cn/rust-static
export RUSTUP_UPDATE_ROOT=https://mirrors.ustc.edu.cn/rust-static/rustup
# 接下来运行命令使文件生效
$ source ~/.bash_profile
```

试了一下还是不行，然后我把翻墙软件重启了一下，再试一遍就好了，所以我也不知道是不是只是因为翻墙软件的原因，简单的来看上面只是增加了一个镜像。两种大家都试一下

安装好了长这样：

![image-20190403150513447](https://github.com/DiDiDaDiDiDa/RUST-/blob/master/docs/images/image-20190403150513447.png)

输入 rustc —version 查看一下版本号

