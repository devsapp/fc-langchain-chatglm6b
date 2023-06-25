
> 注：当前项目为 Serverless Devs 应用，由于应用中会存在需要初始化才可运行的变量（例如应用部署地区、服务名、函数名等等），所以**不推荐**直接 Clone 本仓库到本地进行部署或直接复制 s.yaml 使用，**强烈推荐**通过 `s init ` 的方法或应用中心进行初始化，详情可参考[部署 & 体验](#部署--体验) 。

# fc-langchain-ChatGLM 帮助文档
本项目是以开源[langchain-ChatGLM](https://github.com/imClumsyPanda/langchain-ChatGLM)为基础，将其快速部署到阿里云函数计算上的应用，可以帮助您快速体验chatglm6b的效果。
注意本项目不包含模型部分，其依赖两个模型(.bin后缀的文件)
+ [chatglm6b](https://github.com/THUDM/ChatGLM-6B)
+ [text2vec-large-chinese](https://huggingface.co/GanymedeNil/text2vec-large-chinese)

通过本应用启动的kodbox服务（以admin开头的服务地址）, 分别自行下载到/mnt/auto/chatglm6b/local-chatglm-model 目录
以及/mnt/auto/chatglm6b/local-text2vec-model 下
[构建镜像源码地址](https://github.com/ai-app-with-serverless/langchain-ChatGLM-on-fc)
<description>


</description>

<preview>



</preview>


## 前期准备

使用该项目，您需要有开通以下服务：

<service>



| 服务 |  备注  |
| --- |  --- |
| 函数计算 FC |   |
| 文件存储 NAS |   |

</service>

推荐您拥有以下的产品权限 / 策略：
<auth>
</auth>

<remark>



</remark>

<disclaimers>

免责声明：   
1.应用中心仅为您提供应用的逻辑关系，不为您托管任何资源。如果您部署的应用中，存在一定的资源收费现象，请参考对应产品的收费标准；如果您应用所使用的某些产品或者服务因为产品规划等原因发生了不兼容变更，建议您直接咨询对应的产品或者服务；
2.应用中心为您提供的默认流水线功能是免费的，如果您需要手动切换到自定义流水线可能涉及到资源使用费用，具体的收费标准需要参考函数计算的计费文档；
3.应用中心部署的部分应用会为您分配“devsapp.cn”的测试域名，这个测试域名并非阿里云官方域名，是 CNCF Sandbox 项目 Serverless Devs 所提供的测试域名，我们不保证该域名的使用时效性，推荐您只在测试的时候使用，或者绑定自己的自定义域名进行使用；
4.应用部署过程中，如果提示“当前应用模板由社区贡献，非阿里云官方提供，推荐您在使用当前应用模板前仔细阅读应用详情，以确保应用的安全，稳定等”则表示该应用并非阿里云官方所提供的应用，我们仅作为收录和展示，如果您继续部署该应用，推荐您联系应用的作者，并与作者协商应用使用的相关协议等；

</disclaimers>

## 部署 & 体验

<appcenter>
   
- :fire: 通过 [Serverless 应用中心](https://fcnext.console.aliyun.com/applications/create?template=fc-stable-diffusion) ，
  [![Deploy with Severless Devs](https://img.alicdn.com/imgextra/i1/O1CN01w5RFbX1v45s8TIXPz_!!6000000006118-55-tps-95-28.svg)](https://fcnext.console.aliyun.com/applications/create?template=fc-stable-diffusion) 该应用。
   
</appcenter>
<deploy>
    
- 通过 [Serverless Devs Cli](https://www.serverless-devs.com/serverless-devs/install) 进行部署：
  - [安装 Serverless Devs Cli 开发者工具](https://www.serverless-devs.com/serverless-devs/install) ，并进行[授权信息配置](https://docs.serverless-devs.com/fc/config) ；
  - 初始化项目：`s init fc-stable-diffusion -d fc-stable-diffusion `
  - 进入项目，并进行项目部署：`cd fc-stable-diffusion && s deploy - y`
   
</deploy>

## 应用详情

<appdetail id="flushContent">
</appdetail>

## 使用文档

<usedetail id="flushContent">




</usedetail>


<devgroup>


## 开发者社区

您如果有关于错误的反馈或者未来的期待，您可以在 [Serverless Devs repo Issues](https://github.com/serverless-devs/serverless-devs/issues) 中进行反馈和交流。如果您想要加入我们的讨论组或者了解 FC 组件的最新动态，您可以通过以下渠道进行：

<p align="center">  

| <img src="https://serverless-article-picture.oss-cn-hangzhou.aliyuncs.com/1635407298906_20211028074819117230.png" width="130px" > | <img src="https://serverless-article-picture.oss-cn-hangzhou.aliyuncs.com/1635407044136_20211028074404326599.png" width="130px" > | <img src="https://serverless-article-picture.oss-cn-hangzhou.aliyuncs.com/1635407252200_20211028074732517533.png" width="130px" > |
| --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| <center>微信公众号：`serverless`</center>                                                                                         | <center>微信小助手：`xiaojiangwh`</center>                                                                                        | <center>钉钉交流群：`33947367`</center>                                                                                           |
</p>
</devgroup>
