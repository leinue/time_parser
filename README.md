# timer
An NLP time parser for Chinese

## 背景介绍

时间的处理在人工智能中是比较棘手的一个工作，本模块的目的是使时间的处理简单易用。

## 时间的表达方式

- 大大...前天
- 大前天
- 前天
- 昨天
- 今天
- 明天
- 天
- 大后天
- 大大...后天
- 端午节等各种节日（洋节日、传统节日）
- 在[-3, 6]之间衍生的诸如：明天下午、后天中午、端午节晚上等模糊时间
- 在[-3, 6]之间衍生的诸如：明天下午三点、后天中午12点、端午节晚上0点等精确时间
- 在[-3, 6]之间衍生的诸如：明天下午三点左右、后天中午12点前、端午节晚上0点后等微模糊时间

以上是一阶查询，还有二阶、三阶查询，如：

- 今天的昨天
- 去年的端午节
- 昨天的前天
- 明天的后天
- 去年端午节的前一天(三阶)
