# BeautifulSoup介绍

从HTML和XML文件中提取数据。导航，查找，修改解析数

## 资源

* [官方文档](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
* [中文文档](https://beautifulsoup.readthedocs.io/zh_CN/latest/)

## 解析器

* html.parser python内置标准库，
* lxml 解析HTML，xml 速度快，需要安装C语言库。 推荐使用
* html5lib  以浏览器的方式解析文档，生成HTML5格式的文档，速度慢，不依赖于外部扩展

## 安装

```shell
pip install beautifulsoup4
# 或者
easy_install beautifulsoup4
```

## 对象

HTML文档解析后形成一个复杂的树形结构，每个节点都是pthon对象。分为四类：Tag, NavifableSring, BeautifulSoup

### Tag

* name标签名
* 属性attributes
* 多值属性：返回list

### NavigableString

### BeautifulSoup

### Comment

文档的注释部分

## 遍历文档树

### 子节点

#### tag

#### .contents和.children

#### .descendants

#### .string

#### .strings和stripped_strings

### 父节点

#### .parent

取某个节点的父节点

#### .parents

递归得到元素的所有父辈节点到根节点

### 兄弟节点

#### .next_sibling和.previous_sibling

#### .next_siblings和.previous_siblings

#### .next_element和.previous_element

#### .next_elements和.previous_elments

## 搜索文档树

### find()

返回符合条件的第一个结果

### find_all()

返回符合条件的所有结果

### find_parents()和find_parent()

### find_next_siblings()和find_next_sibling()

### find_previous_siblings()和find_previous_sibling()

### find_all_next()和find_next()

### find_all_previous()和find_previous

### CSS选择器

* tag标签
* 兄弟节点
* 类class
* id
* 属性
* 属性的值
* 组合

## 修改文档树

### 修改tag

### 修改.string

### append()

把新元素添加到父节点

### NavigableString() .new_tag()

### insert()

### insert_before()和insert_after()

### clear()

tag.clear()请吃当前tag的内容

### extract()

tag.extract()将当前tag移除文档树，并作为方法结果返回

### decompose()

tag.decompose()将当前节点移除文档树并完全销毁

### replace_with()

用新tag或者文本替代某断内容

### wrap()

对指定的tag元素进行包装并返回包装后的结果

### unwrap()

移除tag内的所有tag标签

## 输出

格式化输出 prettify()
压缩输出 str() unicode()
