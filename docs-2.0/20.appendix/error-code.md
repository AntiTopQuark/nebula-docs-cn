# 错误码

Nebula Graph 运行出现问题时，会返回错误码。本文介绍错误码的详细信息。

!!! note

    - 如果出现错误但没有返回错误码，或错误码描述不清，请在[论坛](https://discuss.nebula-graph.com.cn/)或 [GitHub](https://github.com/vesoft-inc/nebula/issues) 反馈。
    - 返回`0`表示执行成功。

|错误码|说明|
|:---|:---|
|`-1`| 连接断开 |
|`-2`| 无法建立连接 |
|`-3`| RPC 失败 |
|`-4`| Raft leader 变更|
|`-5`| 图空间不存在 |
|`-6`| Tag 不存在 |
|`-7`| Edge type不存在 |
|`-8`| 索引不存在|
|`-9`| 边属性不存在|
|`-10`| Tag 属性不存在|
|`-11`| 当前角色不存在|
|`-12`| 当前配置不存在|
|`-13`| 当前主机不存在|
|`-15`| listener 不存在|
|`-16`| 当前分区不存在|
|`-17`| key 不存在|
|`-18`| 用户不存在|
|`-19`| 统计信息不存在|
|`-20`| 没有找到当前服务|
|`-21`| drainer 不存在|
|`-22`| drainer 客户端不存在|
|`-24`| 备份失败|
|`-25`| 备份的表为空|
|`-26`| 备份表失败|
|`-27`| multiget 无法获得所有数据|
|`-28`| 重建索引失败|
|`-29`| 密码无效|
|`-30`| 无法获得绝对路径|
|`-1001`| 身份验证失败|
|`-1002`| 无效会话|
|`-1003`| 会话超时|
|`-1004`| 语法错误|
|`-1005`| 执行错误|
|`-1006`| 语句为空|
|`-1008`| 错误的许可证|
|`-1009`| 语义错误|
|`-1010`| 超出最大连接数|
|`-1011`| 访问存储失败（仅有部分请求成功）|
|`-2001`| 主机不存在|
|`-2002`| 主机已经存在|
|`-2003`| 无效主机|
|`-2004`| 当前命令、语句、功能不支持|
|`-2007`| 配置项不能改变|
|`-2008`| 参数与 meta 数据冲突|
|`-2009`| 无效的参数|
|`-2010`| 错误的集群|
|`-2011`| listener 冲突|
|`-2021`| 存储数据失败|
|`-2022`| 存储段非法|
|`-2023`| 无效的数据均衡计划|
|`-2024`| 集群已经处于数据均衡状态|
|`-2025`| 没有正在运行的数据均衡计划|
|`-2026`| 缺少有效的主机|
|`-2027`| 已经损坏的数据均衡计划|
|`-2029`| 缺少有效的 drainer|
|`-2030`| 回收用户角色失败|
|`-2031`| 无效的分区数量|
|`-2032`| 无效的副本因子|
|`-2033`| 无效的字符集|
|`-2034`| 无效的字符排序规则|
|`-2035`| 字符集和字符排序规则不匹配|
|`-2040`| 生成快照失败|
|`-2041`| 写入块数据失败|
|`-2044`| 增加新的任务失败|
|`-2045`| 停止任务失败|
|`-2046`| 保存任务信息失败|
|`-2047`| 数据均衡失败|
|`-2048`| 当前任务还没有完成|
|`-2049`| 任务报表失效|
|`-2050`| 当前任务不在图空间内|
|`-2051`| 当前任务需要恢复|
|`-2065`| 无效的任务|
|`-2066`| 备份终止（正在创建索引）|
|`-2067`| 备份时图空间不存在|
|`-2068`| 备份恢复失败|
|`-2069`| 会话不存在|
|`-2070`| 获取集群信息失败|
|`-2071`| 获取集群信息时无法获取绝对路径|
|`-2072`| 获取集群信息时无法获得 agent|
|`-2073`| query 未找到|
|`-2074`| agent 没有汇报心跳|
|`-2080`| 无效变量|
|`-2081`| 变量值和类型不匹配|
|`-3001`| 选举时无法达成共识|
|`-3002`| key 已经存在|
|`-3003`| 数据类型不匹配|
|`-3004`| 无效的字段值|
|`-3005`| 无效的操作|
|`-3006`| 当前值不允许为空|
|`-3007`| 字段非空或者没有默认值时，字段值必须设置|
|`-3008`| 取值超出了当前类型的范围|
|`-3010`| 数据冲突|
|`-3011`| 写入被延迟|
|`-3021`| 不正确的数据类型|
|`-3022`| VID 长度无效|
|`-3031`| 无效的过滤器|
|`-3032`| 无效的字段更新|
|`-3033`| 无效的 KV 存储|
|`-3034`| peer 无效|
|`-3035`| 重试次数耗光|
|`-3036`| leader 转换失败|
|`-3037`| 无效的统计类型|
|`-3038`| VID 无效|
|`-3040`| 加载元信息失败|
|`-3041`| 生成 checkpoint 失败|
|`-3042`| 生成 checkpoint 被阻塞|
|`-3043`| 数据被过滤|
|`-3044`| 无效的数据|
|`-3045`| 并发写入同一条边发生冲突|
|`-3046`| 并发写入同一个点发生冲突|
|`-3047`| 锁已经失效|
|`-3051`| 无效的任务参数|
|`-3052`| 用户取消了任务|
|`-3053`| 任务执行失败|
|`-3060`| 执行计划被清除|
|`-3070`| 收到请求时心跳流程未完成|
|`-3071`| 收到旧 leader 的过时心跳（已选举出新的 leader）|
|`-3073`| 并发写入时与后到的请求发生冲突|
|`-3061`| 客户端和服务端版本不兼容|
|`-3062`| 获取 ID 序号失败|
|`-3500`| 未知的分区|
|`-3501`| raft 日志落后|
|`-3502`| raft 日志过期|
|`-3503`| 心跳信息已经过期|
|`-3504`| 未知的追加日志|
|`-3511`| 等待快照完成|
|`-3512`| 发送快照过程出错|
|`-3513`| 无效的接收端|
|`-3514`| Raft 没有启动|
|`-3515`| Raft 已经停止|
|`-3516`| 错误的角色|
|`-3521`| 写入 WAL 失败|
|`-3522`| 主机已经停止|
|`-3523`| 请求数量过多|
|`-3524`| 持久化快照失败|
|`-3525`| RPC 异常|
|`-3526`| 没有发现 WAL 日志|
|`-3527`| 主机暂停|
|`-3528`| 写入被堵塞|
|`-3529`| 缓存溢出|
|`-3530`| 原子操作失败|
|`-3531`| leader 租约过期|
|`-3532`| Raft 已经同步数据|
|`-4001`| drainer 日志落后|
|`-4002`| drainer 日志过期|
|`-4003`| drainer 数据存储无效|
|`-4004`| 图空间不匹配|
|`-4005`| 分区不匹配|
|`-4006`| 数据冲突|
|`-4007`| 请求冲突|
|`-4008`| 数据非法|
|`-5001`| 缓存配置错误|
|`-5002`| 空间不足|
|`-5003`| 没有命中缓存|
|`-5005`| 写缓存失败|
|`-7001`| 机器节点数超出限制|
|`-7002`| 解析证书失败|
|`-8000`| 未知错误|

<!--
|`-14`| zone 不存在|
|`-2012`| zone 数量不足|
|`-2013`| Zone 为空|
|`-5004`| |
|`-2043`| |
|`-2006`| |
-->