# 节点安装指引

# 节点部署

系统要求及docker安装指引参考平台安装指引目录。

节点新增部署流程如下：

![Node_deployment](../imgs/node_deployment.png)

## 第 1 步：节点注册-获取节点ID、节点令牌

![Node_step1](../imgs/node_step1.png)

点击节点名称获取：①节点ID、②节点部署令牌

![Node_step2](../imgs/node_step2.png)

![Node_step3](../imgs/node_step3.png)

## 第 2 步：获取Centre平台所在的ip地址-下载并解压部署包-安装部署

若是同一网络内，则只需获取本机的ip地址即可，以mac为例，通过ifconfig命令获取③ip地址。

若是跨网部署，则需要运维人员生成外网IP。

部署包和secretpad的部署包是同一个，所以直接下载解压secretpad的部署包即可。

mac的命令：

1、把解压的安装包拖入到终端（或输入 sercretpad_pkg 的路径）
2、执行 `install.sh` 安装 SecretPad

```shell
cd 部署包所在路径
bash install.sh lite -n alice -m 'https://root-kuscia-master:1080' -t xdeploy-tokenx -p 10080  -k 41802 -g 41803 -s 8180 -q 13181 -P notls
```

![Node_step4](../imgs/node_step4.png)

WSL的命令：

```shell
cd 部署包所在路径
bash install.sh lite -n alice -m 'https://root-kuscia-master:1080' -t xdeploy-tokenx -p 10080  -k 41802 -g 41803 -s 8180 -q 13181 -P notls
```
端口示例：
```
容器:                端口对应:外部->内部  部署参数:
secretpad  http     port:  8088->8080   -s 参数
kuscia     http     prot:  18082->8082  -k 参数
kuscia     grpc     port:  18083->8083  -g 参数
kuscia     gateway  port:  18080->1080  -p 参数
```

配置参数详解：
- n:节点名称，平台页面的计算节点ID
- m:master节点地note
   - 协议:与—P参数对应关系
      - notls->http
      - (tls、mtls)->https
   - ip:master节点的ip地址
   - port:master节点的gateway端口号
- t:节点token，平台页面中的节点部署令牌
- d:项目的安装目录(默认安装目录是：$HOME/kuscia)
- p:参数传递的是 lite/autonomy 容器 kuscia-gateway 映射到主机的端口，保证和主机上现有的端口不冲突即可
- k:参数传递的是 lite/autonomy 容器 Kuscia-api 映射到主机的 HTTP/HTTPS 端口，保证和主机上现有的端口不冲突即可
- g:参数传递的是 lite/autonomy 容器 Kuscia-grpc 映射到主机的 HTTP/HTTPS 端口，保证和主机上现有的端口不冲突即可
- s:secretpad平台端口，保证和主机上现有的端口不冲突即可
- q:参数传递的是 lite/autonomy 容器 kuccia 映射到主机的 env 端口，保证和主机上现有的端口不冲突即可
- P:KusciaAPI 以及节点对外网关使用的通信协议，有三种安全模式可供选择：notls/tls/mtls（非必填，只允许小写，默认：tls)，与 Kuscia 部署配置相同 [protocol参考链接](https://www.secretflow.org.cn/zh-CN/docs/kuscia/v0.6.0b0/deployment/kuscia_config_cn#id3)
   - notls: 此模式下，通信通过未加密的 HTTP 传输，比较安全的内部网络环境或者 Kuscia 已经存在外部网关的情况可以使用该模式【直接部署在公网有安全风险】。
   - tls: (默认)在此模式下，通信通过 TLS 协议进行加密，即使用 HTTPS 进行安全传输，不需要手动配置证书。
   - mtls: 这种模式也使用 HTTPS 进行通信，但它支持双向 TLS 验证，需要手动交换证书以建立安全连接。

需要输入用户名密码，用于登陆节点平台（密码8位，由大小写字母和特殊字符组成）。

![Node_step5](../imgs/node_step5.png)

看到“Lite domain xxxxx deployed successfull”的提示即完成部署

![Node_step6](../imgs/node_step6.png)

## 第 3 步：浏览器访问节点平台

本次新增的节点平台可以直接用浏览器打开 http://localhost：指定端口号 访问，内置的Alice和Bob节点可以直接访问管理数据，新注册的节点需要通过节点平台访问管理数据。

![Node_step7](../imgs/login_img.png)

由于本次新增节点的数据管理功能暂不能直接拖csv文件进行注册，所以需要将文件放到指定目录下才能进行注册，新注册的节点数据管理edge平台界面操作如下：

![Node_step8](../imgs/node_step8.png)

# 数据添加：手动上传文件到服务器指定目录

目前kuscia 使用 docker 部署，docker有磁盘挂载点，算子数据源和结果目前都在 docker容器的/home/kuscia/var/storage/data 目录下

使用命令

```shell
docker ps
```

![Node_step9](../imgs/node_step9.png)

如上图，可以看到宿主机 目录是 /root/kuscia/data/test-inf8eutnhifwod1i

我们就把实体数据文件上传到该目录下

```shell
rz
```

上传文件名字要和创建的时候一致 比如 haha-alice.csv

# 注意事项：机器关闭导致节点不可用

- 若机器关闭重启导致IP改变后节点会变成不可用状态，则需要进到节点的容器里改一下配置将③masterIP改为最新的ip；

- 若新增节点跟master是如果是在一台机器上， 可以设置master的域名，不用ip。 比如https://\${master容器名}:1080

如：找到容器名——输入命令行：`bash install.sh lite -n gmmrgcgt -m 'https://lan-kuscia-master:1080' -t
nNiJL6sKjSmVJUuyj66AK7k6rWT9DMqA -p 30002`——回车即可创建节点成功。

![Node_step10](../imgs/node_step10.png)

# 增加节点用户权限描述

中心化部署模式下，Edge平台成功安装后，可登陆Center平台。Center平台的用户名为计算节点id，密码可通过Edge平台-查看我的节点获取。登录到Center平台，可以看到自己节点的信息和合作项目。Center平台上账号隔离，不可见其他节点信息。