# 历史版本

## 2024年12月
<table>
  <tr>
    <th>类型</th>
    <th>说明</th>
  </tr>
  <tr>
    <th>版本号</th>
    <th>v1.11.0</th>
  </tr>
  <tr>
    <th>更新时间</th>
    <th>2024年12月30日</th>
  </tr>
  <tr>
    <th>更新内容</th>
    <th>新增：
1. 新增自定义SCQL分析组件，支持SecretFlow引擎和SCQL引擎串联，支持多方联合分析
2. 新增三方隐私求交组件
3. 新增单边预处理SQL组件且支持和模型一起打包提交，进行模型发布
4. 模型训练组件支持计算进度展示
优化：
1. 隐私求交组件配置优化
2. woe报告展示各箱的bad_rate、total_rate</th>
  </tr>
  <tr>
    <th>安装包</th>
    <th>[点此下载 x86_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-x86_64-v1.11.0.tar.gz)  
[点此下载 arm_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-aarch_64-v1.11.0.tar.gz)</th>
  </tr>
</table>

版本映照关系
<table>
  <tr>
    <th>模块</th>
    <th>版本</th>
  </tr>
  <tr>
    <th>SecretpPad</th>
    <th>0.12.0b0</th>
  </tr>
  <tr>
    <th>Kuscia</th>
    <th>0.13.0b0</th>
  </tr>
  <tr>
    <th>SecretFlow</th>
    <th>1.11.0b1</th>
  </tr>
  <tr>
    <th>Serving</th>
    <th>0.8.0b0</th>
  </tr>
  <tr>
    <th>dataproxy</th>
    <th>0.3.0b0</th>
  </tr>
  <tr>
    <th>scql</th>
    <th>0.9.2b1</th>
  </tr>
</table>

## 2024年11月
<table>
  <tr>
    <th>类型</th>
    <th>说明</th>
  </tr>
    <tr>
    <th>版本号</th>
    <th>v1.10.0</th>
  </tr>
  <tr>
    <th>更新时间</th>
    <th>2024年11月4日</th>
  </tr>
  <tr>
    <th>更新内容</th>
    <th>新增：
1. SecretPad建模画布支持定时周期任务创建、查看和管理 ，可按分区读取 odps 数据源
2. 数据新增 MySQL 数据源，支持多样化场景数据接入
3. 画布组件库新增读模型、模型回测算子
4. 新增了 Prometheus 常规监控指标，默认关闭
5. 数据按字段授权到项目优化</th>
  </tr>
  <tr>
    <th>安装包</th>
    <th>[点此下载 x86_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-x86_64-v1.10.0.tar.gz)  
[点此下载 arm_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-aarch_64-v1.10.0.tar.gz)</th>
  </tr>
</table>

版本映照关系
<table>
  <tr>
    <th>模块</th>
    <th>版本</th>
  </tr>
  <tr>
    <th>SecretpPad</th>
    <th>0.11.0b0</th>
  </tr>
  <tr>
    <th>Kuscia</th>
    <th>0.12.0b0</th>
  </tr>
  <tr>
    <th>SecretFlow</th>
    <th>1.10.0b0/1.10.0b1</th>
  </tr>
  <tr>
    <th>Serving</th>
    <th>0.7.0b0</th>
  </tr>
  <tr>
    <th>dataproxy</th>
    <th>0.2.0b0</th>
  </tr>
</table>


## 2024年8月
<table>
  <tr>
    <th>类型</th>
    <th>说明</th>
  </tr>
    <tr>
    <th>版本号</th>
    <th>v1.9.0</th>
  </tr>
  <tr>
    <th>更新时间</th>
    <th>2024年08月30日</th>
  </tr>
  <tr>
    <th>更新内容</th>
    <th>新增：
1. 支持部署并管理多计算节点，支持用户隔离研发和生产环境
2. 新增ODPS数据源，并支持模型发布到oss、odps数据源
3. 支持在新增数据时，对空值进行自定义
4. 隐私求交组件支持数据仅输出导某一方
5. 行级过滤算子支持过滤空值行</th>
  </tr>
  <tr>
    <th>安装包</th>
    <th>[点此下载 x86_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-x86_64-v1.9.0.tar.gz)  
[点此下载 arm_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-aarch_64-v1.9.0.tar.gz)</th>
  </tr>
</table>

版本映照关系
<table>
  <tr>
    <th>模块</th>
    <th>版本</th>
  </tr>
  <tr>
    <th>SecretpPad</th>
    <th>0.10.0b0/0.10.1b0</th>
  </tr>
  <tr>
    <th>Kuscia</th>
    <th>0.11.0b0</th>
  </tr>
  <tr>
    <th>SecretFlow</th>
    <th>1.9.0b0/1.9.0b2</th>
  </tr>
  <tr>
    <th>Serving</th>
    <th>0.6.0b0</th>
  </tr>
  <tr>
    <th>dataproxy</th>
    <th>0.1.0b1</th>
  </tr>
</table>

## 2024年7月
<table>
  <tr>
    <th>类型</th>
    <th>说明</th>
  </tr>
    <tr>
    <th>版本号</th>
    <th>v1.8.0</th>
  </tr>
  <tr>
    <th>更新时间</th>
    <th>2024年07月30日</th>
  </tr>
  <tr>
    <th>更新内容</th>
    <th>新增：
1. SecureBoost训练支持tweedie回归，并支持early stop</th>
  </tr>
  <tr>
    <th>安装包</th>
    <th>[点此下载 x86_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-x86_64-v1.8.0.tar.gz)  
[点此下载 arm_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-aarch_64-v1.8.0.tar.gz)</th>
  </tr>
</table>

版本映照关系
<table>
  <tr>
    <th>模块</th>
    <th>版本</th>
  </tr>
  <tr>
    <th>SecretpPad</th>
    <th>0.9.0b0</th>
  </tr>
  <tr>
    <th>Kuscia</th>
    <th>0.10.0b0</th>
  </tr>
  <tr>
    <th>SecretFlow</th>
    <th>1.8.0b0</th>
  </tr>
  <tr>
    <th>Serving</th>
    <th>0.5.0b0</th>
  </tr>
</table>

## 2024年6月
<table>
  <tr>
    <th>类型</th>
    <th>说明</th>
  </tr>
    <tr>
    <th>版本号</th>
    <th>v1.7.0</th>
  </tr>
  <tr>
    <th>更新时间</th>
    <th>2024年07月02日</th>
  </tr>
  <tr>
    <th>更新内容</th>
    <th>新增：
1. 新增类型转换、采样、评分卡转换、人群稳定性评估组件
2. 新增数据源管理，支持增删改查；并新增支持OSS数据源
3. 支持画布粒度配置默认存储数据源
优化：
1. Easy PSI漏洞修复</th>
  </tr>
  <tr>
    <th>安装包</th>
    <th>[点此下载 x86_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-x86_64-v1.7.0.tar.gz)  
[点此下载 arm_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-aarch_64-v1.7.0.tar.gz)
</th>
  </tr>
</table>

版本映照关系
<table>
  <tr>
    <th>模块</th>
    <th>版本</th>
  </tr>
  <tr>
    <th>SecretpPad</th>
    <th>0.8.0b0/0.8.1b0</th>
  </tr>
  <tr>
    <th>Kuscia</th>
    <th>0.9.0b0</th>
  </tr>
  <tr>
    <th>SecretFlow</th>
    <th>1.7.0b0</th>
  </tr>
  <tr>
    <th>Serving</th>
    <th>0.4.0b0</th>
  </tr>
</table>

## 2024年5月
<table>
  <tr>
    <th>类型</th>
    <th>说明</th>
  </tr>
    <tr>
    <th>版本号</th>
    <th>v1.6.0</th>
  </tr>
  <tr>
    <th>更新时间</th>
    <th>2024年05月15日</th>
  </tr>
  <tr>
    <th>更新内容</th>
    <th>新增：
1. 广义线性回归模型支持P值评估
2. onehot组件支持丢弃众数枚举值后入模，从而实现众数列作为入模特征的base组
3. 逻辑回归训练组件增加是否输出模型报告配置，从而可输出入模特征权重
4. 增加union组件，支持同节点样本表或联合表横向拼接
5. 新增平台组件线性模型参数修改（目前支持广义线性回归模型修改），并支持模型打包、发布
6. 集成阿里云SLS，web界面展示SLS各组件详细日志
7. 画布展示组件版本
8. 模型发布时可指定系统cpu、内存的上下限
优化：
1. 隐私求交组件配置优化
2. 优化单元测试结构、日志输出内容和格式</th>
  </tr>
  <tr>
    <th>安装包</th>
    <th>[点此下载 x86_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-x86_64-v1.6.0.tar.gz)  
[点此下载 arm_64 安装包](https://secretflow-public.oss-cn-hangzhou.aliyuncs.com/mvp-packages/secretflow-allinone-linux-aarch_64-v1.6.0.tar.gz)</th>
  </tr>
</table>

版本映照关系
<table>
  <tr>
    <th>模块</th>
    <th>版本</th>
  </tr>
  <tr>
    <th>SecretpPad</th>
    <th>0.7.1b0/0.7.2b0</th>
  </tr>
  <tr>
    <th>Kuscia</th>
    <th>0.8.0b0</th>
  </tr>
  <tr>
    <th>SecretFlow</th>
    <th>1.6.1b0</th>
  </tr>
  <tr>
    <th>Serving</th>
    <th>0.3.1b0</th>
  </tr>
</table>


## 2024年4月
<table>
  <tr>
    <th>类型</th>
    <th>说明</th>
  </tr>
    <tr>
    <th>版本号</th>
    <th>v1.5.0</th>
  </tr>
  <tr>
    <th>更新时间</th>
    <th>2024年04月15日</th>
  </tr>
  <tr>
    <th>更新内容</th>
    <th>新增：
1. 完善P2P模式下平台引擎日志，日志模块支持阿里云SLS
2. 支持MySQL数据源，并提供MySQL 数据库的支持文档
优化：
1. 优化平台隐私求交组件，支持 left join、full join等
2. 更改组件连线，统计类型组件支持输入表
3. 画布运行时性能优化
4. 修复画布时运行时有项目参与方未提供数据时的运行失败问题
5. 修复组件选择时未清除状态问题</th>
  </tr>
  <tr>
    <th>安装包</th>
    <th></th>
  </tr>
</table>

版本映照关系
<table>
  <tr>
    <th>模块</th>
    <th>版本</th>
  </tr>
  <tr>
    <th>SecretpPad</th>
    <th>0.6.0b0</th>
  </tr>
  <tr>
    <th>Kuscia</th>
    <th>0.7.0b0</th>
  </tr>
  <tr>
    <th>SecretFlow</th>
    <th>1.5.0b0</th>
  </tr>
  <tr>
    <th>Serving</th>
    <th>0.2.1b0</th>
  </tr>
</table>

## 2024年3月
<table>
  <tr>
    <th>类型</th>
    <th>说明</th>
  </tr>
    <tr>
    <th>版本号</th>
    <th>v1.4.0</th>
  </tr>
  <tr>
    <th>更新时间</th>
    <th>2024年03月23日</th>
  </tr>
  <tr>
    <th>更新内容</th>
    <th>新增：
1. 支持模型在线预测
2. 增加模型管理模块，支持查看打包的模型列表
3. 增加 http 数据源，并支持模型发布关联 http 数据进行离在线特征映射
优化：
1. 广义线性回归模型性能优化、增加分箱修改、模型预测组件优化、隐私求交组件支持left join、full join等
2. 日志优化，数据同步优化降低资源消耗</th>
  </tr>
  <tr>
    <th>安装包</th>
    <th></th>
  </tr>
</table>

版本映照关系
<table>
  <tr>
    <th>模块</th>
    <th>版本</th>
  </tr>
  <tr>
    <th>SecretpPad</th>
    <th>0.5.0b0</th>
  </tr>
  <tr>
    <th>Kuscia</th>
    <th>0.6.0b0</th>
  </tr>
  <tr>
    <th>SecretFlow</th>
    <th>1.4.0b0</th>
  </tr>
  <tr>
    <th>Serving</th>
    <th>0.2.0b0</th>
  </tr>
</table>


## 2024年1月
<table>
  <tr>
    <th>类型</th>
    <th>说明</th>
  </tr>
    <tr>
    <th>版本号</th>
    <th>v1.3.0</th>
  </tr>
  <tr>
    <th>更新时间</th>
    <th>2024年01月11日</th>
  </tr>
  <tr>
    <th>更新内容</th>
    <th>新增：
1. 平台支持 P2P 部署架构，支持从端侧发起项目合作，不依赖可信第三方
2. 节点路由创建支持 P2P 模式
3. P2P部署模式的平台下，项目合作需要对方同意，且增加项目存档能力
4. P2P部署模式的平台下，增加工作台模块，快速查看我要处理的事项和我的项目
优化：
1. 存量组件增加配置参数，便于更灵活构造训练任务
2. P2P 模式下平台项目创建需要受邀方审批同意
3. 模型预测（SecureBoost）组件优化，支持分批预测
4. 整体 UI 更新</th>
  </tr>
  <tr>
    <th>安装包</th>
    <th></th>
  </tr>
</table>

版本映照关系
<table>
  <tr>
    <th>模块</th>
    <th>版本</th>
  </tr>
  <tr>
    <th>SecretpPad</th>
    <th>0.3.0b0</th>
  </tr>
  <tr>
    <th>Kuscia</th>
    <th>0.4.0b0</th>
  </tr>
  <tr>
    <th>SecretFlow</th>
    <th>1.3.0.dev20231109</th>
  </tr>
</table>