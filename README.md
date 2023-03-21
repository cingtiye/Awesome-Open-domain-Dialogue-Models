# Awesome Open-domain Dialogue Models

受益于人工智能的技术突破和产品落地，对话系统在⼯业界的应⽤呈爆炸式增⻓，本仓库主要收集目前网上公开的一些高质量开放域对话模型（感谢分享资源的个人、团队以及企业），并将持续更新......

**注**: :sweat_smile: [huggingface](https://github.com/huggingface/transformers)模型下载地址: 1. [huggingface官方地址](https://huggingface.co/models)

# Expand Table of Contents
+ [中文开放域对话数据集](#中文开放域对话数据集)
+ [中文对话模型](#中文对话模型)
  - [CDial-GPT系列](#CDial-GPT系列)
  - [EVA系列](#EVA系列)
  - [ChatLLM系列](#ChatLLM系列)
  - [PLATO系列](#PLATO系列)
  - [PanGu系列](#PanGu系列)
  - [OPD](#OPD)
  - [Sky系列](#Sky系列)
  - [MOSS](#MOSS)
  - [ChatYuan](#ChatYuan)
+ [英文对话模型](#英文对话模型)
  - [Blender系列](#Blender系列)
  - [LaMDA](#LaMDA)
  - [ChatGPT](#ChatGPT)

## 中文开放域对话数据集

- <a name="LCCC">LCCC</a> | 文本 |2020 | LCCC数据集分为base和large两个版本，主要用于预训练大规模对话生成模型，其base版本包括了12M个对话，32.9M个对话语句 | [`PDF`](https://arxiv.org/abs/2008.03946) | [`数据链接`](https://github.com/thu-coai/CDial-GPT)
- PchatbotW | 文本 | 2021 | PchatbotW主要从微博爬取得到，包括了139,448,339个对话、 278,896,678，并且提供了时间戳和用户ID两种个性信息，可以隐式地建模说话者的个性 | [`PDF`](https://arxiv.org/abs/2009.13284) | [`数据集链接`](https://github.com/qhjqhj00/Pchatbot)
- WDC-Dialogue | 文本 | 2021 | WDC是一个超大规模的中文对话数据集，其平均轮次为2.1，包括了1.4B个对话，以及3.0B个语句 | [`PDF`](https://arxiv.org/pdf/2108.01547.pdf) | [`数据集链接`](https://resource.wudaoai.cn/home?ind&name=WuDaoCorpora%202.0&id=1394901288847716352)
- M3ED | 多模态 | 2022 | M3ED构建了一个大规模高质量的多模态、多场景、多标签情感对话数据集，从56部中文电视剧，大约500集中选取900多个对话片段，并对对话中的每句话进行多情感标签的标注，共标注24,449句话 | [`PDF`](https://aclanthology.org/2022.acl-long.391/) | [`数据链接`](https://github.com/aim3-ruc/rucm3ed)
- CPED | 多模态 | 2022 | CPED由与情感和个性相关的多源知识组成，包括性别、人格特征、13种情绪、19种对话行为和10个场景，包含超过12K段对话 | [`PDF`](https://arxiv.org/pdf/2205.14727v1.pdf) | [`数据链接`](https://github.com/scutcyr/CPED)
- C3KG | 文本 | 2022 |C3KG是第一个结合了社会常识知识和对话流信息的中文常识对话知识图谱 | [`PDF`](https://arxiv.org/pdf/2204.02549.pdf) | [`数据链接`](https://github.com/XiaoMi/C3KG)
- MMChat | 多模态 | 2022 | MMChat是一个大规模多模态多轮对话数据集，其中的每个对话都与一个或多个图片相关联 | [`PDF`](https://arxiv.org/pdf/2108.07154.pdf) | [`数据集链接`](https://github.com/silverriver/MMChat)
- 千言中文对话数据集 | 文本 | 千言中文对话数据集包括DeLeMon、Diamante、LUGE-Dialogue、DuConv、DuRecDial、KdConv、PersonaDialog等，内容涵盖闲聊对话、情感对话、画像对话、知识对话、推荐对话等多个方面 | [`PDF`](https://www.luge.ai/#/luge/about) |  [`数据集链接`](https://www.luge.ai/#/)
- <a name="GlobalWoZ">GlobalWoZ</a> | 文本 | 2022 | GlobalWoZ是利用机器翻译和目标语言的本地实体创建一个新的多语言大规模ToD数据集GlobalWoZ | [`PDF`](https://aclanthology.org/2022.acl-long.115.pdf) | [`数据链接`](https://ntunlpsg.github.io/project/globalwoz/)
- <a name="TikTalk">TikTalk</a> | 多模态 | 2023 | TikTalk数据集从抖音上采集，其抖音拥有超过25个大类的视频，包括38703个视频和相应367670个对话 |  [`PDF`](https://arxiv.org/pdf/2301.05880.pdf) | [`数据链接`](https://github.com/RUC-AIMind/TikTalk)

## 中文对话模型

### CDial-GPT系列

| 模型 | 版本 | PyTorch | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |
| CDial-GPTLCCC-base  | base | [huggingface](https://huggingface.co/thu-coai/CDial-GPT_LCCC-base) | [thu-coai](https://github.com/thu-coai)         | [CDial-GPT](https://github.com/thu-coai/CDial-GPT)       |  中文对话  |
| CDial-GPT2LCCC-base | base | [huggingface](https://huggingface.co/thu-coai/CDial-GPT2_LCCC-base) | [thu-coai](https://github.com/thu-coai)| [CDial-GPT](https://github.com/thu-coai/CDial-GPT)           |  中文对话 |
| CDial-GPTLCCC-large | large | [huggingface](https://huggingface.co/thu-coai/CDial-GPT_LCCC-large) | [thu-coai](https://github.com/thu-coai)         | [CDial-GPT](https://github.com/thu-coai/CDial-GPT)           | 中文对话 |
| GPT2-dialogue       |  base    | <p>[Google Drive](https://drive.google.com/drive/folders/1Ogz3eapvtvdY4VUcY9AEwMbNRivLKhri?usp=sharing)</br>[百度网盘-osi6](https://pan.baidu.com/s/1qDZ24VKLBU9GKARX9Ev65g)</p> | [yangjianxin1](https://github.com/yangjianxin1) | [GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat) |  闲聊对话 |
| GPT2-mmi  | base  | <p>[Google Drive](https://drive.google.com/drive/folders/1oWgKXP6VG_sT_2VMrm0xL4uOqfYwzgUP?usp=sharing)</br>[百度网盘-1j88](https://pan.baidu.com/s/1ubXGuEvY8KmwEjIVTJVLww)</p> | [yangjianxin1](https://github.com/yangjianxin1) | [GPT2-chitchat](https://github.com/yangjianxin1/GPT2-chitchat) |  闲聊对话 |

### EVA系列

+ 2021 | EVA: An Open-Domain Chinese Dialogue System with Large-Scale Generative Pre-Training | Hao Zhou, et al. | arXiv | [`PDF`](https://arxiv.org/abs/2108.01547)
+ 2022 | EVA2.0: Investigating Open-Domain Chinese Dialogue Systems with Large-Scale Pre-Training | Yuxian Gu, et al. | arXiv | [`PDF`](https://arxiv.org/pdf/2203.09313.pdf)

| 模型 | 版本 | 介绍 | 模型下载 | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| EVA |  28亿参数 | [项目首页](https://wudaoai.cn/model/detail/EVA) | [模型下载](https://wudaoai.cn/model/download?resourceId=1428554651225075712&filename=eva-ckpt.tar.gz) | [thu-coai](https://github.com/thu-coai) | [github](https://github.com/thu-coai/EVA) | 中文开放域对话  |
| EVA2.0-xLarge |  xlarge | [项目首页](https://wudaoai.cn/model/detail/EVA) | [huggingface](https://huggingface.co/thu-coai/EVA2.0-xlarge) | [thu-coai](https://github.com/thu-coai) | [github](https://github.com/thu-coai/EVA) | 中文开放域对话  |  
| EVA2.0-large |  large | [项目首页](https://wudaoai.cn/model/detail/EVA) | [huggingface](https://huggingface.co/thu-coai/EVA2.0-large) | [thu-coai](https://github.com/thu-coai) | [github](https://github.com/thu-coai/EVA) | 中文开放域对话  |  
| EVA2.0-base |  base | [项目首页](https://wudaoai.cn/model/detail/EVA) | [huggingface](https://huggingface.co/thu-coai/EVA2.0-base) | [thu-coai](https://github.com/thu-coai) | [github](https://github.com/thu-coai/EVA) | 中文开放域对话  |  

### ChatLLM系列

| 模型    | 版本 | 介绍                                             | 模型下载                                               | 作者                                   | 源地址                                         | 应用领域       |
| ------- | ---- | ------------------------------------------------ | ------------------------------------------------------ | -------------------------------------- | ---------------------------------------------- | -------------- |
| ChatGLM | 6B   | [项目首页](https://chatglm.cn/blog)              | [huggingface](https://huggingface.co/THUDM/chatglm-6b) | [THUDM](https://github.com/THUDM)      | [github](https://github.com/THUDM/ChatGLM-6B)  | 中英开放域对话 |
| BELLE   | 7B   | [项目首页](https://github.com/LianjiaTech/BELLE) | [huggingface](https://huggingface.co/BelleGroup)       | [贝壳](https://github.com/LianjiaTech) | [github](https://github.com/LianjiaTech/BELLE) | 中英开放域对话 |

### PLATO系列

:thinking: <a name="PLATO-XL">体验地址</a>: 手机微信搜索**百度PLATO**即可体验 (**目前已失效**)

:thinking: <a name="ERNIE Bot">体验地址</a>: [ERNIE Bot](https://yiyan.baidu.com/) 

- 2020 | PLATO: Pre-trained Dialogue Generation Model with Discrete Latent Variable | Siqi Bao, et al. | arxiv | [`PDF`](https://arxiv.org/pdf/1910.07931.pdf)

- 2021 | PLATO-2: Towards Building an Open-Domain Chatbot via Curriculum Learning | Siqi Bao, et al. | arxiv | [`PDF`](https://arxiv.org/pdf/2006.16779.pdf)

- 2021 | PLATO-XL: Exploring the Large-scale Pre-training of Dialogue Generation | Siqi Bao, et al. | arxiv | [`PDF`](https://arxiv.org/pdf/2109.09519.pdf) 
- 2022 | PLATO-KAG: Unsupervised Knowledge-Grounded Conversation via Joint Modeling | Xinxian Huang, et al. | aclanthology | [`PDF`](https://aclanthology.org/2021.nlp4convai-1.14.pdf)
- 2022 | Long Time No See! Open-Domain Conversation with Long-Term Persona Memory | Xinchao Xu, et al. | arxiv | [`PDF`](https://arxiv.org/pdf/2203.05797.pdf)
- 2022 | <a name="PLATO-K">PLATO-K</a>: Internal and External Knowledge Enhanced Dialogue Generation | Siqi Bao, et al. | arxiv | [`PDF`](https://arxiv.org/pdf/2211.00910.pdf)

| 模型 | 版本 | 介绍 | 模型下载 | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| PLATO | base | [项目地址](https://github.com/PaddlePaddle/Research/tree/master/NLP/Dialogue-PLATO) |  | [PaddlePaddle](https://github.com/PaddlePaddle) | [github](https://github.com/PaddlePaddle/Research/tree/master/NLP/Dialogue-PLATO) | 中文开放域对话 |
| PLATO-2 | 93M | [项目地址](https://github.com/PaddlePaddle/Knover) |  | [PaddlePaddle](https://github.com/PaddlePaddle) | [github](https://github.com/PaddlePaddle/Knover/tree/develop/projects/PLATO-2) | 中文开放域对话 |
| PLATO-2 | 314M | [项目地址](https://github.com/PaddlePaddle/Knover) | | [PaddlePaddle](https://github.com/PaddlePaddle) | [github](https://github.com/PaddlePaddle/Knover/tree/develop/projects/PLATO-2) | 中文开放域对话 |
| PLATO-2 | 1.6B | [项目地址](https://github.com/PaddlePaddle/Knover) | | [PaddlePaddle](https://github.com/PaddlePaddle) | [github](https://github.com/PaddlePaddle/Knover/tree/develop/projects/PLATO-2) | 中文开放域对话 |
| PLATO-XL | 11B | [项目地址](https://github.com/PaddlePaddle/Knover) |  | [PaddlePaddle](https://github.com/PaddlePaddle) | [github](https://github.com/PaddlePaddle/Knover/tree/develop/projects/PLATO-XL) | 中文开放域对话 |
| PLATO-KAG | 1.6B | [项目地址](https://github.com/PaddlePaddle/Knover) |  | [PaddlePaddle](https://github.com/PaddlePaddle) | [github](https://github.com/PaddlePaddle/Knover/tree/develop/projects/PLATO-KAG) | 中文知识型对话 |
| PLATO-LTM | 1.6B | [项目地址](https://github.com/PaddlePaddle/Research/tree/master/NLP) |  | [PaddlePaddle](https://github.com/PaddlePaddle) | [github](https://github.com/PaddlePaddle/Research/tree/master/NLP/ACL2022-DuLeMon) | 中文开放域对话 |
| PLATO-K | 22B |  | | [PaddlePaddle](https://github.com/PaddlePaddle) |  | 中文开放域对话 |
| ERNIE Bot |  | | |  | | 中英开放域对话 |

### PanGu系列

- 2022 | PANGU-BOT: Efficient Generative Dialogue Pre-training from Pre-trained Language Model | Fei Mi, et al | arxiv | [`PDF`](https://arxiv.org/pdf/2203.17090.pdf)
- 2023 | PanGu-Σ: Towards Trillion Parameter Language Model with Sparse Heterogeneous Computing | Xiaozhe Ren, et al | arxiv | [`PDF`](https://arxiv.org/abs/2303.10845)

| 模型 | 版本 | 介绍 | 模型下载 | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| PanGu-bot | 350M | [项目首页](https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Dialog) |  | [huawei-noah](https://github.com/huawei-noah) | [github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/PanGu-Bot) | 中文开放域对话 |
| PanGu-bot | 2.6B | [项目首页](https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Dialog) | [模型下载](https://openi.pcl.ac.cn/PCL-Platform.Intelligence/PanGu-Dialog#user-content-4-1-%E6%A8%A1%E5%9E%8B%E6%96%87%E4%BB%B6:~:text=4%20%E4%BD%BF%E7%94%A8-,4.1%20%E6%A8%A1%E5%9E%8B%E6%96%87%E4%BB%B6,-%E6%A8%A1%E5%9E%8B%E6%96%87%E4%BB%B6) | [huawei-noah](https://github.com/huawei-noah) |  [github](https://github.com/huawei-noah/Pretrained-Language-Model/tree/master/PanGu-Bot)  | 中文开放域对话 |
| PANGU-$\sum$ | 1.085T |  |  | [huawei-noah](https://github.com/huawei-noah) |  | 中文开放域对话 |

### OPD

| 模型 | 版本 | 介绍 | 模型下载 | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| OPD |  6.3B | [项目首页](http://coai.cs.tsinghua.edu.cn/static/opd/) | [模型下载](http://coai.cs.tsinghua.edu.cn/static/opd/) | [thu-coai](https://github.com/thu-coai) | [github](https://github.com/thu-coai/OPD) | 中文开放域对话  | 需要申请才能下载 |

### Sky系列

| 模型    | 版本 | 介绍                                                         | 模型下载                                                     | 作者                                      | 源地址                                                       | 应用领域         |
| ------- | ---- | ------------------------------------------------------------ | ------------------------------------------------------------ | ----------------------------------------- | ------------------------------------------------------------ | ---------------- |
| SkyText | 2.6B | [项目首页](https://live.vhall.com/v3/lives/subscribe/697547540) | [模型下载](https://huggingface.co/SkyWork/SkyTextTiny)       | [SkyWork](https://huggingface.co/SkyWork) | [github](https://github.com/SkyWorkAIGC/SkyText)             | 中文GPT3支持对话 |
| SkyText | 13B  | [项目首页](https://live.vhall.com/v3/lives/subscribe/697547540) | [模型下载](https://huggingface.co/SkyWork/SkyText/tree/main) | [SkyWork](https://huggingface.co/SkyWork) | [github](https://github.com/SkyWorkAIGC/SkyText)             | 中文GPT3支持对话 |
| SkyChat | -    | [项目首页](https://github.com/SkyWorkAIGC/SkyChat-CN-Chatbot-GPT3/blob/main/README.CN.md) | -                                                            | [SkyWork](https://huggingface.co/SkyWork) | [github](https://github.com/SkyWorkAIGC/SkyChat-CN-Chatbot-GPT3) | 中文GPT3对话     |

### MOSS

:thinking:体验地址：[moss](https://moss.fastnlp.top/)

| 模型 | 版本 | 介绍                                                    | 模型下载                                                | 作者                                        | 源地址           | 应用领域 |
| ---- | ---- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------- | ---------------- | -------- |
| MOSS | 百亿级别 | [项目首页](https://txsun1997.github.io/blogs/moss.html) | [模型下载](https://github.com/txsun1997/MOSS) | [复旦大学自然语言处理实验室](https://nlp.fudan.edu.cn/) | [github](https://github.com/txsun1997/MOSS) |中文ChatGPT|

### ChatYuan

:thinking:体验地址：[ChatYuan](http://www.clueai.cn/chat)

| 模型     | 版本     | 模型大小 | 介绍                                                         | 模型下载                                                    | 作者                                 | 源地址                                        | 应用领域             |
| -------- | -------- | -------- | ------------------------------------------------------------ | ----------------------------------------------------------- | ------------------------------------ | --------------------------------------------- | -------------------- |
| ChatYuan | large-v1 | 770M     | [项目首页](https://mp.weixin.qq.com/s/-axa6XcjGl_Koeq_OrDq8w) | [模型下载](https://huggingface.co/ClueAI/ChatYuan-large-v1) | [ClueAI](https://github.com/clue-ai) | [github](https://github.com/clue-ai/ChatYuan) | 元语功能型对话大模型 |

## 英文对话模型

### Blender系列

:thinking: <a name="Blender">体验地址</a>(目前仅支持US用户):  [BlenderBot](https://geo-not-available.blenderbot.ai/)

- 2021 | BlenderBot 2.0: An open source chatbot that builds long-term memory and searches the internet | Moya Chen, et al. | parl.ai | [`PDF`](https://parl.ai/projects/blenderbot2/)

- 2022 | BlenderBot 3: a deployed conversational agent that continually learns to
  responsibly engage | Kurt Shuster | arxiv | [`PDF`](https://arxiv.org/pdf/2208.03188.pdf)

| 模型 | 版本 | 介绍 | 模型下载 | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| BlenderBot 2.0 | 400M | [项目地址](https://parl.ai/projects/blenderbot2/) | [模型下载](https://parl.ai/projects/blenderbot2/) | [ParIAI](https://parl.ai/) | [blenderbot2](https://parl.ai/projects/blenderbot2/) | 英文开放域对话 |
| BlenderBot 2.0 | 2.7B |  [项目地址](https://parl.ai/projects/blenderbot2/) | [模型下载](https://parl.ai/projects/blenderbot2/)  | [ParIAI](https://parl.ai/) | [blenderbot2](https://parl.ai/projects/blenderbot2/) | 英文开放域对话 |
| BlenderBot 3.0 | 3B |  [项目地址](https://ai.facebook.com/blog/blenderbot-3-a-175b-parameter-publicly-available-chatbot-that-improves-its-skills-and-safety-over-time/) | [模型下载](https://parl.ai/projects/bb3/) | [ParIAI](https://parl.ai/) | [blenderbot3](https://ai.facebook.com/blog/blenderbot-3-a-175b-parameter-publicly-available-chatbot-that-improves-its-skills-and-safety-over-time/) | 英文开放域对话 |
| BlenderBot 3.0 | 30B |  [项目地址](https://ai.facebook.com/blog/blenderbot-3-a-175b-parameter-publicly-available-chatbot-that-improves-its-skills-and-safety-over-time/) | [模型下载](https://parl.ai/projects/bb3/) | [ParIAI](https://parl.ai/) | [blenderbot3](https://ai.facebook.com/blog/blenderbot-3-a-175b-parameter-publicly-available-chatbot-that-improves-its-skills-and-safety-over-time/) | 英文开放域对话 |
| BlenderBot 3.0 | 175B | [项目地址](https://ai.facebook.com/blog/blenderbot-3-a-175b-parameter-publicly-available-chatbot-that-improves-its-skills-and-safety-over-time/) | [模型下载](https://docs.google.com/forms/d/e/1FAIpQLSfRzw8xVzxaxgRyuodTZtkcYADAjzYjN5gcxx6DMa4XaGwwhQ/viewform) |  [ParIAI](https://parl.ai/) |[blenderbot3](https://ai.facebook.com/blog/blenderbot-3-a-175b-parameter-publicly-available-chatbot-that-improves-its-skills-and-safety-over-time/)  | 英文开放域对话 |

### LaMDA
:thinking: <a name="LaMDA">体验地址</a>(支持中英等多种语言): [Character.AI](https://beta.character.ai/chats/)

- 2022 | LaMDA: Language Models for Dialog Applications | Romal Thoppilan, et al. | arxiv | [`PDF`](https://arxiv.org/pdf/2201.08239.pdf)

| 模型 | 版本 | 介绍 | 模型下载 | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| LaMDA | 2B | [项目地址](https://ai.googleblog.com/2022/01/lamda-towards-safe-grounded-and-high.html) | - | - | [LaMDA-pytorch](https://github.com/conceptofmind/LaMDA-pytorch) |  英文开放域对话 |
| LaMDA | 8B |[项目地址](https://ai.googleblog.com/2022/01/lamda-towards-safe-grounded-and-high.html) | - | - | [LaMDA-pytorch](https://github.com/conceptofmind/LaMDA-pytorch) | 英文开放域对话 |
| LaMDA | 137B | [项目地址](https://ai.googleblog.com/2022/01/lamda-towards-safe-grounded-and-high.html) | - | - | [LaMDA-pytorch](https://github.com/conceptofmind/LaMDA-pytorch) | 英文开放域对话 |

### ChatGPT

:thinking:体验地址（支持中英等多种语言）参考网站：[参考](https://blog.ittutorial.top/ai-ChatGPT/)

- 2022 | Training language models to follow instructions with human feedback | Long Ouyang, et al. | arxiv | [`PDF`](https://arxiv.org/pdf/2203.02155.pdf)
- 2023 | GPT-4 Technical Report | OpenAI* | [`PDF`](https://cdn.openai.com/papers/gpt-4.pdf)

| 模型 | 版本 | 介绍 | 模型下载 | 作者| 源地址 | 应用领域 |
| ---- | ---- | ---- | ---- | ---- | ---- |---- |
| ChatGPT | - | [项目地址](https://openai.com/blog/chatgpt/) | - | [OpenAI](https://github.com/openai) | [ChatGPT](https://openai.com/blog/chatgpt/) | 通用生成模型 |
| InstructGPT | - | [项目地址](https://github.com/openai/following-instructions-human-feedback) | - | [OpenAI](https://github.com/openai) | [InstructGPT](https://openai.com/blog/instruction-following/#guide) | 通用生成模型 |
| GPT4 | - | [项目地址](https://openai.com/product/gpt-4) | - | [OpenAI](https://github.com/openai) | [GPT4](https://openai.com/research/gpt-4) | 通用生成模型 |


## Reference

[1] [常见对话生成数据集整理](https://www.cxymm.net/article/m0_37201243/120051649#IEMOCAP_6)

[2] [Awesome Pretrained Chinese NLP Models](https://github.com/lonePatient/awesome-pretrained-chinese-nlp-models)

[3] [千言中文对话](https://www.luge.ai/#/)

## 更新
* 2023.03.21 增加<a href='#PanGu系列'>PANGU-$\sum$</a>，PANGU-$\sum$是一个在Ascend 910 AI处理器和MindSpore框架的集群上训练的一个万亿参数的语言模型
* 2023.03.21 增加<a href='#ChatLLM系列'>BELLE</a>，BELLE是一个开源的中文对话大模型，基于Stanford Alpaca，并对中文做了优化
* 2023.03.20 增加<a href='#PLATO系列'>ERNIE Bot</a>，ERNIE Bot是百度团队发布的一个人工智能语言模型，中文名是文心一言，可以回答用户的问题，为用户提供有用的信息，并帮助用户完成创作
* 2023.03.15 增加<a href="#ChatGPT">GPT4</a>，GPT-4是OpenAI最先进的模型，能够产生更安全、更有用的回复
* 2023.03.14 增加<a href='#ChatLLM系列'>ChatGLM</a>， ChatGLM是一个开源的、支持中英双语的对话语言模型，是一个初具问答和对话功能的千亿中英语言模型
* 2023.03.06 增加<a href='#ChatYuan'>ChatYuan</a>，ChatYuan是业内首个功能型对话开源中文大模型，可以用于回答问题、可以结合上下文做对话、做各种生成任务，包括创意性写作，也能回答法律、新冠等领域类问题
* 2023.02.21 增加<a href='#MOSS'>MOSS</a>，MOSS是复旦大学自然语言处理实验室发布的一个具备 ChatGPT 能力的语言模型
* 2023.01.31 增加<a href="#TikTalk">TikTalk</a>，TikTalk是一个真实闲聊中文多模态数据集，共包括38703个视频和相应367670个对话
* 2022.12.27 增加<a href="#Sky系列">SkyChat</a>, SkyChat是一款基于中文GPT-3 API研发的聊天机器人项目，它除了基本的聊天、对话、你问我答外，还能支持中英文互译、内容续写、对对联、写古诗、生成菜谱、第三人称转述、创建采访问题等多种功能
* 2022.12.19 增加<a href="#Sky系列">SkyText</a>，SkyText是由奇点智源发布的中文GPT3预训练大模型，可以进行聊天、问答、中英互译等不同的任务
* 2022.12.13 增加<a href="#ChatGPT">InstructGPT</a>，InstructGPT和ChatGPT在模型结构，训练方式上都完全一致，都采用了指示学习和人工反馈的强化学习来指导模型的训练
* 2022.12.04 增加<a href="#ChatGPT">ChatGPT</a>，ChatGPT是一个由 OpenAI 训练的大型语言模型，ChatGPT 支持和用户通过对话的形式“回答问题”，并且赋予了一些简单的智能化行为
* 2022.11.23 增加<a href="#PLATO-K">PLATO-K</a>，PLATO-K提出了同时结合知识内化和知识外用的全面知识增强策略，参数规模达到了220亿，是当前最大规模的中文对话模型
* 2022.11.17 增加<a href="#GlobalWoZ">GlobalWoZ</a>，GlobalWoZ是面向全球通用的人机对话系统多语言任务型对话数据
* 2022.11.16 增加<a href="#PLATO-XL">PLATO-XL</a>、<a href="#LaMDA">LaMDA</a>a和<a href="#Blender">Blender</a>体验地址，可以与闲聊机器人面对面聊天
* 2022.11.09 增加[OPD](#OPD)，OPD是一个中文开放域对话预训练模型，拥有63亿参数，在70GB高质量对话数据上进行训练而成
* 2022.11.04 增加[LaMDA](#LaMDA)，LaMDA 通过微调一系列专门用于对话的、基于 Transformer 的神经语言模型构建的，具有多达 137B 个参数，模型还可以利用外部知识源进行对话
* 2022.10.25 增加[Blender系列模型](#Blender系列)，Facebook下一系列对话模型
* 2022.10.15 增加[PanGu系列模型](#PanGu系列)，PanGu-Dialog是以大数据和大模型为显著特征的大规模开放域对话生成模型，充分利用大规模预训练语言模型的知识和语言能力，构建可控、可靠可信、有智慧的自然人机对话模型
* 2022.09.30 增加[PLATO系列模型](#PLATO系列)，百度自主研发的集闲聊、任务、知识于一身的对话机器人
* 2022.09.25 增加[EVA系列模型](#EVA系列)，EVA 是目前最大的开源中文预训练对话模型
* 2022.09.17 初始化中文[CDial-GPT系列模型](#CDial-GPT系列)，最早开源的中文对话模型，同时还开源了闲聊对话数据集<a href="#LCCC">LCCC</a>
* 2022.08.17 增加[中文开放域对话数据集](#中文开放域对话数据集)