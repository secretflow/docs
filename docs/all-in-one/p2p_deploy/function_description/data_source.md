# 数据源管理

## 1. 模块说明

本模块主要是对节点自有数据源进行管理，包括数据源增删改查，当前仅支持OSS数据源；本地文件和HTTTP数据在数据管理添加数据即可

## 2. 注册数据源
在数据源管理页面，点击注册数据：
![Data1](../../imgs/data_source1.png)
### 需输入
- 平台展示的名字，即显示名称 
- endpoint名称
- AcessKeyID
- AcessKeySecret
- virtualhost 
  - 阿里云的oss需要打开这个virtualhost；其余minio等不需要
- bucket
- 预设路径（可选）
- 节点连接配置