 <h1 align="center">InternLM大语言模型</h1>
  <p align="center">
    <a href="README.md"><strong>English</strong></a> | <strong>简体中文</strong>
  </p>


## 目录

- [仓库简介](#项目介绍)
- [前置条件](#前置条件)
- [镜像说明](#镜像说明)
- [获取帮助](#获取帮助)
- [如何贡献](#如何贡献)

## 项目介绍

[InternLM](https://github.com/InternLM/InternLM) 是由上海人工智能实验室（Shanghai AI Laboratory）开发的高性能多模态大语言模型系列。本商品基于arm架构的Huawei Cloud EulerOS 2.0 64bit系统，提供开箱即用的InternLM2.5-1.8B-Chat模型。

## 主要特点

- 使用上万亿高质量语料，建立模型超强知识体系；
- 支持8k语境窗口长度，实现更长输入与更强推理体验；
- 通用工具调用能力，支持用户灵活自助搭建流程；
- 提供了支持模型预训练的轻量级训练框架，无需安装大量依赖包，一套代码支持千卡预训练和单卡人类偏好对齐训练，同时实现了极致的性能优化，实现千卡训练下近90%加速效率。

本项目提供的开源镜像商品 [**InternLM大语言模型**](https://marketplace.huaweicloud.com/contents/91ef08ac-85b7-4092-85cb-46bef1c805ba#productid=OFFI1121281402292875264) 已预先安装InternLM2.5-1.8B-Chat及其相关运行环境，并提供部署模板。快来参照使用指南，轻松开启“开箱即用”的高效体验吧。


> **系统要求如下：**
> - CPU: 4vCPUs 或更高
> - RAM: 16GB 或更大
> - Disk: 至少 40GB

## 前置条件
[注册华为账号并开通华为云](https://support.huaweicloud.com/usermanual-account/account_id_001.html)

## 镜像说明

| 镜像规格                                                                                                                           | 特性说明 | 备注 |
|--------------------------------------------------------------------------------------------------------------------------------| --- | --- |
| [internlm2_5-1_8b-chat-kunpeng](https://github.com/HuaweiCloudDeveloper/InternLM-image/tree/internlm2_5-1_8b-chat-kunpeng) | 基于鲲鹏服务器 + Huawei Cloud EulerOS 2.0 64bit 安装部署 |  |

## 获取帮助
- 更多问题可通过 [issue](https://github.com/HuaweiCloudDeveloper/InternLM-image/issues) 或 华为云云商店指定商品的服务支持 与我们取得联系
- 其他开源镜像可看 [open-source-image-repos](https://github.com/HuaweiCloudDeveloper/open-source-image-repos)

## 如何贡献
- Fork 此存储库并提交合并请求
- 基于您的开源镜像信息同步更新 README.md
