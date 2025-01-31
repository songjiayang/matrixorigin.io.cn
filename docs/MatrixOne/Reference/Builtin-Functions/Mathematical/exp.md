# **EXP()**

## **函数说明**

EXP(number)函数返回以自然常数e为底的number的指数。

## **函数语法**

```
> EXP(number)
```

## **参数释义**

|  参数   | 说明  |
|  ----  | ----  |
| number | 必要参数，可取任意数值数据类型 |

## **示例**

```sql
drop table if exists t1;
create table t1(a int ,b float);
insert into t1 values(-4, 2.45);
insert into t1 values(6, -3.62);

mysql> select exp(a), exp(b) from t1;
+---------------------+----------------------+
| exp(a)              | exp(b)               |
+---------------------+----------------------+
| 0.01831563888873418 |   11.588347271798835 |
|   403.4287934927351 | 0.026782679557672436 |
+---------------------+----------------------+
2 rows in set (0.00 sec)
```
