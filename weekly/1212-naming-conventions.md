---
aliases:
  - 命名约束
created: 2024-11-02T12:00:00
status:
  - writing/draft
modified: 2024-12-24T09:22:52
---

不知不觉，传到 OneDrive 的数据已经有 324G。加上大学四年乱八七糟的课业，网络随处搜集来的二手文档，他们虽然看似错综复杂，但极细斟酌的话，你又会发现，其实其实仍然存在着某种顺序，但这无益，只会让他们显得更加杂乱无章。

从某种意义上来说，这就是屎山。

![](https://raw.githack.com/bGZo/assets/dev/2024/20241102201058.png)


很早就看到过牛津大学的一篇文章 https://datamanagement.hms.harvard.edu/plan-design/file-naming-conventions ，我落实在了工作的文档中，以如下格式命名：

$$YYYYDDMM-Project-Name-Version.format$$

这启发于上述文章中提供的一些方法论：

- 构建你的规则
    - 你现在有那些组的文件？
    - 不同组（项目/学科）可以采用完全迥异的命名规则；
    - 如果已有相关规则，遵守即可；
- 找到元数据 (metadata)
    - 在计算机中，开头第一个名字最重要，找到你想检索用的名字，他们可以是：
        - 数据类型
        - 合作人姓名
        - 地点
        - 时间 (YYYYMMDD)
    - 文件名应该是描述性的，并提供足够的上下文信息。
- 缩写元数据
    - 决定哪些保持元数据；
    - 用 2/3 个字符替代它；
    - 记录这些被缩写的代码；
- 版本控制
    - 可以用 时间/递增 字典序追加在文件后；
- 想想要如何搜索
    - 像【元数据】中说的，第一顺位非常重要；
- 分割不同元数据
    - 建议采用 `-`
- 记录下你的命名规则；

当然，此处的启发同样适用于 [[index]] 中提到的命名约束。

希望对你有启发。