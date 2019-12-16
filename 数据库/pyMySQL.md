# pyMySQL

[pyMySQL](https://github.com/PyMySQL/PyMySQL)，[文档](https://pymysql.readthedocs.io/en/latest/modules/connections.html) pyMySQ共有两个对象Connection和Cursor。

## 安装pymysql

```python
pip3 install PyMySQL
```

## Connection

### close()

关闭数据库连接

### commit()

提交修改

### rollback()

回滚

## Cursor

游标

### excute()

执行SQL语句

### fetchone()

获取下一个查询结果集，结果集是一个对象

### fetchall()

接收全部的返回结果行

### rowcount()

返回执行execute()方法后影响的行数

### cursor.close()

关闭游标

## 使用方法

### 连接数据库

```python
import pymysql

conn = pymysql.connect(host="localhost",
                       port=3306,
                       user="root",
                       passwd="Tcsd1234",
                       db="pytest")
```
