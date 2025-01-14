# months_sub

## 功能

从日期中减去指定的月数。

## 语法

```Haskell
DATETIME months_sub(DATE|DATETIME expr1,INT expr2);
```

## 参数说明

`expr1`: 指定的日期，支持的数据类型为 DATETIME 或 DATE。

`expr2`: 被减去的月数，支持的数据类型为 INT。

## 返回值说明

返回值的数据类型为 DATETIME。

## 示例

```Plain Text
select months_sub('2022-02-28 15:04:05', 1);
+--------------------------------------+
| months_sub('2022-02-28 15:04:05', 1) |
+--------------------------------------+
| 2022-01-28 15:04:05                  |
+--------------------------------------+

select months_sub('2022-02-28', 1);
+-----------------------------+
| months_sub('2022-02-28', 1) |
+-----------------------------+
| 2022-01-28 00:00:00         |
+-----------------------------+
```
