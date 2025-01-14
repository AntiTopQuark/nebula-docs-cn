# NebulaGraph Analytics License

License 是为用户提供的软件授权证书。用户在部署 NebulaGraph Analytics 时，需要设置 License 才能正常启动 NebulaGraph Analytics。本文介绍 NebulaGraph Analytics 的 License 相关信息。

## 注意事项

- 没有设置 License 时，NebulaGraph Analytics 无法启动。

- 请勿修改 License，否则会导致 License 失效。

- License 快过期时，请[联系我们](https://www.nebula-graph.com.cn/contact)申请续期。
  
- License 的过期缓冲为 14 天：
  
  - 过期前 30 天和过期当天，服务启动时会打印日志进行提醒。
  
  - 过期后仍可继续使用 14 天。
  
  - 过期 14 天后，服务无法启动，并会打印日志进行提醒。

## 获取方式

[联系我们](https://www.nebula-graph.com.cn/contact)申请 NebulaGraph Analytics License。

!!! note

    填写 [NebulaGraph Analytics 试用申请](https://wj.qq.com/s2/10158890/69a8)可获取 30 天免费试用的 License。

## NebulaGraph Analytics License 说明

NebulaGraph Analytics License 是一个名为`nebula.license`的文件，内容示例如下：

```bash
----------License Content Start----------
{
  "vendor": "vesoft",
  "organization": "vesoft",
  "issuedDate": "2022-11-01T16:00:00.000Z",
  "expirationDate": "2023-11-01T15:59:59.000Z",
  "product": "nebula_graph_analytics",
  "version": ">3.0.0",
  "licenseType": "enterprise",
  "gracePeriod": 14,
  "analytics": {
    "nodes": 3,
    "vcpu": 3
  }
  "clusterCode": "BAIAEAiAQAAG"
}
----------License Content End----------

----------License Key Start----------
Rrjip5c+xxxxxxxxxxxxxk5Yg==
----------License Key End----------
```

License 文件包含生效时间、过期时间等信息。说明如下。

|参数|说明|
|:---|:---|
|`vendor`| 发放渠道。|
|`organization`| 用户名称。|
|`issuedDate`| License 生效时间。|
|`expirationDate`| License 过期时间。|
|`product`| 产品类型。NebulaGraph Analytics 的产品类型为`nebula_graph_analytics`。|
|`version`| 版本支持的信息。|
|`licenseType`| License 类型（预留参数）。包括`enterprise`、`samll_bussiness`、`pro`、`individual`。|
|`gracePeriod`| 证书过期后可继续使用服务的缓冲时间（单位天），超过缓冲期后停止服务。试用版的 License 过期后无缓冲期，默认值为 0。 |
|`nodes`|集群中 Analytics 服务的数量限制。|
|`vcpu`|集群中 Analytics 服务的总线程数量限制。|
|`clusterCode`| 用户的硬件信息，也是集群的唯一标识码。试用版的 License 中无此参数。 |

## 使用方式

关于如何使用 NebulaGraph Analytics License，参见[NebulaGraph Analytics](nebula-analytics.md)。

## 续期操作

按照以下操作续期 NebulaGraph Analytics License。

1. [联系我们](https://www.nebula-graph.com.cn/contact)申请新的 NebulaGraph Analytics License 文件`nebula.license`。
2. 在 NebulaGraph Analytics 的安装目录下（例如，`/usr/local/nebula-analytics/scripts/`），使用新的 License 文件替换旧的 License 文件。

!!! note

    NebulaGraph Analytics License 过期后，用户无法正常使用 Analytics。为了保证业务正常运行，请及时更新 License。
