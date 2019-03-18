
连接MySQL出现 `ModuleNotFoundError: No module named 'MySQLdb'` 错误

## step

### 换成 pymysql 

只要在配置SQLALCHEMY_DATABASE_URI时，加上一个pymysql就可以了： 

```
app.config['SQLALCHEMY_DATABASE_URI'] = 'mysql+pymysql://root:dzd123@localhost/你的数据库名' 
```

当然，前提是要已经安装了pymysql:

- 如果没有装pymysql，是会报ModuleNotFoundError: No module named 'pymysql'错误的
- 安装命令也很简单：pip install pymysql

### (未成功)安装库 


https://blog.csdn.net/qq_36523839/article/details/80569420

根据你自己的系统安装下面的库来解决问题：

```
easy_install mysql-python (mix os)
pip install mysql-python (mix os)
apt-get install python-mysqldb (Linux Ubuntu)
cd/usr/ports/databases/py-MySQLdb && make install clean (FreeBSD)
yum install MySQL-python (linux Fedora, CentOS)
pip install mysqlclient (Windows)
```
安装后一般没有问题，如果还有报错，那么肯定问题不止这一个，你可能还缺少其它的功能。

## ref
- https://blog.csdn.net/qq_25046261/article/details/78991442
