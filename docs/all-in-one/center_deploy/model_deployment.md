# 快速完成模型发布

进行前置准备：模型训练和模型评估后，可进行模型和预处理规则的打包，并将打包后的模型进行模型发布操作。

## Step1：添加HTTP数据

如仅进行模型发布体验，可跳过此步骤，平台在模型发布环节内置mock特征进行体验。

![Step1.1](../imgs/model_deployment_center1.png)

点击添加数据-HTTP数据后，需输入SPI数据地址、数据表名称和描述，并上传或填写数据表schame进行数据添加。

![Step1.2](../imgs/model_deployment2.png)

## Step2：模型提交

完成一个建模任务后，且画布中有运行成功状态的模型时，可点击模型提交进行模型打包：

![Step2.1](../imgs/model_deployment3.png)

点击提交模型后，选择一个训练好的模型，此时系统会自动关联模型的预处理规则，此时填写模型名称和描述，点击“确认提交”可完成模型的打包提交，并在模型管理模块查看此模型。

![Step2.2](../imgs/model_deployment4.png)

## Step3：模型发布

模型提交后，可在模型管理进行模型查看和模型发布，点击模型发布后，可进行模型的离在线特征映射：

![Step3.1](../imgs/model_deployment5.png)

系统内置mock特征，如需使用真实的特征服务，需要前置注册http特征并授权到该项目 <font color=#DF2A3F>（此处中心化部署模式下暂不支持）。</font>

![Step3.2](../imgs/model_deployment6.png)

点击确定后，模型即可发布成功，可查看模型，并使用模型ID和endpoints构建特征服务API，详见：https://www.secretflow.org.cn/zh-CN/docs/kuscia/v0.6.0b0/tutorial/run_sf_serving_with_api_cn

![Step3.3](../imgs/model_deployment7.png)


