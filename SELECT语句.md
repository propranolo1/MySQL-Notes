# SELECT语句

SELECT [列1,列2,...] FROM [表]

不同的列使用逗号进行隔开

## 查询整张表的内容

使用*号

```mysql
SELECT * FROM employees;
```

## 列的别名

1.直接空格写出别名名称

2.添加AS

3.使用双引号""

```mysql
SELECT [列的名称] [列的别名]  FROM [表];
SELECT [列的名称] AS [列的别名]  FROM [表];
SELECT [列的名称] "列的别名" FROM [表];
```

## 去除重复的行(DISTINCT)

```mysql
SELECT DISTINCT 列 FROM 表;
```

![image-20220804085815104](https://propran-img.oss-cn-hangzhou.aliyuncs.com/img/image-20220804085815104.png)

![image-20220804085900496](https://propran-img.oss-cn-hangzhou.aliyuncs.com/img/image-20220804085900496.png)

## 空值参与运算

空值null

null不同于0

如果使用了空值参与运算，则运算结果也为空值

## 着重号

如果该字段和语法冲突，或和保留字相同

则需要使用``

##  查询常数（待完善

```
SELECT '常数'
```

## 显示表结构

可以显示表字段中的详细信息

```mysql
DESCRIBE 表名;
DESC 表名; #二者效果相同
```

![image-20220804085622333](https://propran-img.oss-cn-hangzhou.aliyuncs.com/img/image-20220804085622333.png)

## 过滤数据

```mysql
 SELECT *
FROM [表名]
WHERE [列名][运算符][数字];
```

![image-20220804090956090](https://propran-img.oss-cn-hangzhou.aliyuncs.com/img/image-20220804090956090.png)