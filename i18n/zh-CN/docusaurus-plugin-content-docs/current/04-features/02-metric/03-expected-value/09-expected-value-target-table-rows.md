---
id: 'expected-value-target-table-rows'
title: '期望值-目标表总行数'
---

## 概念解释
`目标表总行数` 期望值类型表示在数据质量检查过程中使用的期望值是计算检查的目标表的总行数。

## 使用方法
- 点击创建规则作业，选择数据质量作业
- 在期望值中选择 `目标表总行数`。

## 计算方式
- 相关参数
    - uniqueKey：会根据每个规则的配置信息生成一个唯一键值,为8位长度的字符串

- `Local`&`Spark`&`Livy` 引擎
```
select count(1) as expected_value_${uniqueKey} from ${target_table}
``` 

## 使用案例

### 场景
...

### 思路
...

### 步骤
...