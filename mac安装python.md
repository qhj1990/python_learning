# Mac安装python

Mac系统本身自带python2.X的版本，

## mac安装python的方法

### 系统自带python

系统自带python, 可执行以下代码判断是否已经安装好python，以及python的版本

### 1. brew 安装python

```shell
brew install python3
```

安装后执行

```shell
python3 --version
```

可确认是否安装完成python3

### 2.官网下载pkg安装包

[python官网](python.org) download python 3.x, 下载完成后双击运行即完成python的安装

## python多版本管理

很多老项目都是python2.x, 然而现在推荐的python版本都是3.x, 两者不完全兼容。这时可能会需要安装多个版本的python, 并在不同的版本之间进行切换。

### pyenv

pyenv [github](https://github.com/pyenv/pyenv)

1. 安装pyenv

```shell
brew install pyenv
```

2. 安装多个版本python

```shell
```

3. 切换不同的版本

4. pyenv其他命令

```shell
pyenv unistall 3.8.0 # 卸载python
brew uninstall pyenv # 卸载pyenv
```

## 不同版本可能产生的问题

1. pycharm终端运行时，可能会报错 "ModuleNotFoundError: No module named 'XXXXXX' ".
