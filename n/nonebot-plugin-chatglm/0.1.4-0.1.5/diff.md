# Comparing `tmp/nonebot-plugin-chatglm-0.1.4.tar.gz` & `tmp/nonebot-plugin-chatglm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatglm-0.1.4.tar", last modified: Wed Mar 22 14:33:26 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatglm-0.1.5.tar", last modified: Sat Apr 22 06:55:49 2023, max compression
```

## Comparing `nonebot-plugin-chatglm-0.1.4.tar` & `nonebot-plugin-chatglm-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1066 2023-03-16 08:48:31.448425 nonebot-plugin-chatglm-0.1.4/LICENSE
--rw-r--r--   0        0        0     9283 2023-03-22 14:31:47.781696 nonebot-plugin-chatglm-0.1.4/README.md
--rw-r--r--   0        0        0  2467981 2023-03-21 08:51:11.149269 nonebot-plugin-chatglm-0.1.4/nonebot_plugin_chatglm/20B_tokenizer.json
--rw-r--r--   0        0        0      371 2023-03-22 14:32:51.665443 nonebot-plugin-chatglm-0.1.4/nonebot_plugin_chatglm/__init__.py
--rw-r--r--   0        0        0     2963 2023-03-22 14:18:45.588891 nonebot-plugin-chatglm-0.1.4/nonebot_plugin_chatglm/chat.py
--rw-r--r--   0        0        0     1343 2023-03-22 14:13:00.166325 nonebot-plugin-chatglm-0.1.4/nonebot_plugin_chatglm/config.py
--rw-r--r--   0        0        0      600 2023-03-21 06:09:26.691996 nonebot-plugin-chatglm-0.1.4/nonebot_plugin_chatglm/help.py
--rw-r--r--   0        0        0     2965 2023-03-22 12:01:11.287515 nonebot-plugin-chatglm-0.1.4/nonebot_plugin_chatglm/mini_rwkv.py
--rw-r--r--   0        0        0      732 2023-03-22 14:33:05.721387 nonebot-plugin-chatglm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     9614 1970-01-01 00:00:00.000000 nonebot-plugin-chatglm-0.1.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1066 2023-03-30 15:44:54.648609 nonebot-plugin-chatglm-0.1.5/LICENSE
+-rwxr-xr-x   0        0        0    12696 2023-04-22 04:50:27.051728 nonebot-plugin-chatglm-0.1.5/README.md
+-rwxr-xr-x   0        0        0      385 2023-04-21 15:13:10.903495 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/__init__.py
+-rwxr-xr-x   0        0        0     5333 2023-04-21 14:59:24.873870 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/chat.py
+-rwxr-xr-x   0        0        0     2739 2023-04-21 14:57:14.093043 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/config.py
+-rw-r--r--   0        0        0      645 2023-04-21 13:59:19.386536 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/prompt.py
+-rwxr-xr-x   0        0        0     2277 2023-04-21 15:05:45.988139 nonebot-plugin-chatglm-0.1.5/nonebot_plugin_chatglm/utils.py
+-rwxr-xr-x   0        0        0      732 2023-04-22 05:01:22.373097 nonebot-plugin-chatglm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    13027 1970-01-01 00:00:00.000000 nonebot-plugin-chatglm-0.1.5/PKG-INFO
```

### Comparing `nonebot-plugin-chatglm-0.1.4/LICENSE` & `nonebot-plugin-chatglm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatglm-0.1.4/README.md` & `nonebot-plugin-chatglm-0.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,117 @@
-<p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
-</p>
+Metadata-Version: 2.1
+Name: nonebot-plugin-chatglm
+Version: 0.1.5
+Summary: 基于ChatGLM-6B的NoneBot2插件
+License: MIT
+Author-email: dao_mingze <dao_mingze@163.com>
+Requires-Python: >=3.8
+Project-URL: repository, https://github.com/DaoMingze/zhukebot/tree/main/zhukebot/plugins/chatglm
+Description-Content-Type: text/markdown
 
 <div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="200" height="200" alt="nonebot"></a>
+<br/><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 
 # nonebot-plugin-chatglm
 
 _✨ NoneBot [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) 支持插件 ✨_
 
-![licese](https://img.shields.io/github/license/DaoMingze/zhukebot)
-![Python](https://img.shields.io/badge/python-3.9+-blue)
+![python](https://img.shields.io/badge/python-3.8+-blue)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DaoMingze/zhukebot/main.svg)](https://results.pre-commit.ci/latest/github/DaoMingze/zhukebot/main)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
-![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm)
+[![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm)](https://pypi.org/project/nonebot-plugin-chatglm)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm)
+![nonebot](https://img.shields.io/badge/nonebot-2-red)
+![onebot](https://img.shields.io/badge/onebot-11-white)
+![licese](https://img.shields.io/github/license/DaoMingze/zhukebot)
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot?ref=badge_shield)
 
 </div>
 
 ## 介绍
 
-使用[ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B)为后端，[NoneBot2](https://github.com/nonebot/nonebot2)为平台的极其简单的本地中文（汉语） AI chat 插件。
+使用 [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) 为后端，[NoneBot2](https://github.com/nonebot/nonebot2) 为平台的极其简单的本地中文（汉语） AI chat 插件。
+
+首次加载等待时间视 Hugging Face 下载速度而定。
+
+## [更新说明](changelog.md)
+
+如有其他功能需求或疑问，欢迎提 issues，当然如果您实现了某些功能或修复了问题，也非常欢迎您提 PR。
+
+### 待办
+
+- [ ] 限制记忆轮数（~~在抄了，在抄了~~）
+- [ ] 图片输出功能（nonebot-plugin-htmlrender）（~~在抄了，在抄了~~）
+- [ ] 管理员在线配置
+  - [ ] 增加写入读取本地配置文件（json）以实现配置的在线热更新
+- [ ] @[Bot] 机器人 使用功能（调试阶段，我个人不太需要，不过后续加上吧）
+
+### 办结/功能
+
+- [x] 完善的默认配置，开箱即用。
+- [x] 模型自动下载并存放到指定位置（HuggingFace Hub提供）
+- [x] 保存对话记录以实现多轮对话
+- [x] 冷却时间（根据测试效果，默认 30 秒）
+- [x] 配置角色功能，基本实现
 
 ### 环境要求
 
-| 量化等级 | 最低显存 |
-| :------: | :------: |
-|   FP16   |   13GB   |
-|   INT8   |   10GB   |
-|   INT4   |   6GB    |
+<div align="center">
+
+| 量化等级       | 推理       | 微调 |                       策略 |
+| -------------- | ---------- | ---- | -------------------------: |
+| 无             | CPU        |      |                   .float() |
+| FP16（无量化） | 13GB 显存  | 14GB |             .half().cuda() |
+| INT8           | 8GB 显存   | 9GB  | .half().quantize(8).cuda() |
+| INT4           | 6GB 显存   | 7GB  | .half().quantize(4).cuda() |
+| INT4 模型      | 5.2GB 显存 |      |             .half().cuda() |
+| INT4-QE 模型   | 4.3GB 显存 |      |             .half().cuda() |
+
+</div>
+
+现在默认使用 CPU 推理，方便开箱即用，但速度较慢。
 
-使用 INT4 量化后的[模型](https://huggingface.co/THUDM/chatglm-6b-int4)。需要 4.2 GB 左右的存储空间（模型），NVIDIA 显卡（使用 CUDA）、6G 及以上的显存。现在默认使用 CPU 推理，方便开箱即用，但速度较慢。
+硬件需求上：训练>微调>推理，但本插件仅考虑推理应用场景。
 
-> 实际可以低于 Python 3.9（但 none-adapter-onebot 要求 Python 3.8+）。
+> none-adapter-onebot 要求 Python 3.8+
 
 ## 安装与更新
 
 ### 软件环境
 
+指除去 Python 和 nonebot 以外的软件环境
+
 #### CUDA
 
-- Windows：见[CUDA 官方文档|英文](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html)
-- Linux：见[CUDA 官方文档|英文](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html)
+- Windows：见 [CUDA 官方文档 | 英文](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html)
+- Linux：见 [CUDA 官方文档 | 英文](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html)
 
 #### PyTorch
 
-见[PyTorch 官方导引](https://pytorch.org/get-started/locally/)
+见 [PyTorch 官方导引](https://pytorch.org/get-started/locally/)
 
 ### 插件
 
 <details>
 <summary><b>（一）使用 nb-cli 安装与更新</b></summary>
 
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+在 nonebot2 项目的根目录下打开命令行，输入以下指令即可安装
 
 ```bash
 nb plugin install nonebot-plugin-chatglm --upgrade
 ```
 
 </details>
 
 <details>
 
 <summary><b>（二）使用包管理器安装与更新</b></summary>
-1、在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令：
+1、在 nonebot2 项目的插件目录下，打开命令行，根据你使用的包管理器，输入相应的安装命令：
 <details>
 <summary>pip</summary>
 
 ```bash
 pip install nonebot-plugin-chatglm
 ```
 
@@ -90,121 +137,162 @@
 
 ```bash
 conda install nonebot-plugin-chatglm
 ```
 
 </details>
 
-2、打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+2、打开 nonebot2 项目根目录下的 `pyproject.toml` 文件，在 `[tool.nonebot]` 部分追加写入
 
 ```toml
 plugins = ["nonebot_plugin_chatglm"]
 ```
 
 </details>
 
-## 配置
+## 配置与依赖
 
 ### ChatGLM 模型
 
-> 模型简介：ChatGLM-6B 是一个开源的、支持中英双语的对话语言模型，基于[General Language Model (GLM) ](https://github.com/THUDM/GLM) 架构，具有 62 亿参数。结合模型量化技术，用户可以在消费级的显卡上进行本地部署（INT4 量化级别下最低只需 6GB 显存）。 ChatGLM-6B 使用了和 ChatGPT 相似的技术，针对中文问答和对话进行了优化。经过约 1T 标识符的中英双语训练，辅以监督微调、反馈自助、人类反馈强化学习等技术的加持，62 亿参数的 ChatGLM-6B 已经能生成相当符合人类偏好的回答。
+> 模型简介：ChatGLM-6B 是一个开源的、支持中英双语的对话语言模型，基于 [General Language Model (GLM)](https://github.com/THUDM/GLM) 架构，具有 62 亿参数。结合模型量化技术，用户可以在消费级的显卡上进行本地部署（INT4 量化级别下最低只需 6GB 显存）。 ChatGLM-6B 使用了和 ChatGPT 相似的技术，针对中文问答和对话进行了优化。经过约 1T 标识符的中英双语训练，辅以监督微调、反馈自助、人类反馈强化学习等技术的加持，62 亿参数的 ChatGLM-6B 已经能生成相当符合人类偏好的回答。
 
-默认使用`HuggingFace Hub`加载，即如果没有设置路径，则会自动下载到用户目录下的`.cache/huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4`。
+#### 选择模型
 
-- 如果是较小显存（< 10 G）且只用聊天对话模型（ChatGLM-6B-INT4）[^1]则没用必要修改。
-- 如果使用 6B 完整模型，则可以自行设置路径。
+<div align="center">
 
-模型的具体使用，还请关注[原仓库说明](https://github.com/THUDM/ChatGLM-6B)提交检测 →![GitHub last commit](https://img.shields.io/github/last-commit/THUDM/ChatGLM-6B?style=flat-square)
+ChatGLM-6B 系列模型
 
-[^1]: 在其他位置配置量化后的 INT4 模型，发生一些编译错误，暂时~~懒得~~没有能力解决。
+| 模型名称                                                              | 量化情况                            | 权重大小 |
+| --------------------------------------------------------------------- | ----------------------------------- | -------: |
+| [ChatGLM-6B](https://huggingface.co/THUDM/chatglm-6b)                 | 无                                  |  13.73GB |
+| [ChatGLM-6B-INT4](https://huggingface.co/THUDM/chatglm-6b-int4)       | INT4: GLM Block                     |   4.06GB |
+| [ChatGLM-6B-INT4-QE](https://huggingface.co/THUDM/chatglm-6b-int4-qe) | INT4: GLM Block, Embedding, LM Head |   3.13GB |
 
-手动下载：
+</div>
+
+- 如果是较小显存（< 10 G）且只用聊天对话模型（ChatGLM-6B-INT4-QE）[^1] 则没用必要修改。
+- 如果使用 6B 完整模型，则可以自行设置路径。
 
-→[清华云盘](https://cloud.tsinghua.edu.cn/d/fb9f16d6dc8f482596c2/)（仅模型文件，是 6B 完整模型，显存较小需要量化使用，暂未设置，需要自行在`chat.py`文件中修改）
+[^1]: 在其他位置配置量化后的 INT4 模型，发生一些编译错误，暂时~~懒得~~没有能力解决。
 
-→[🤗 Hugging Face](https://huggingface.co/THUDM/chatglm-6b-int4)（完整文件），约 4.2 GB。
+#### 下载模型
 
-### ChatRWKV 模型
+默认使用`HuggingFace Hub`加载，即如果没有设置路径，则会自动下载到用户目录下的`.cache/huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4-qe`，可以通过下面的代码转移模型。
 
-> 模型简介：ChatRWKV is like ChatGPT but powered by my RWKV (100% RNN) language model, which is the only RNN (as of now) that can match transformers in quality and scaling, while being faster and saves VRAM.
->
-> ChatRWKV 是一个由[@PENG Bo](https://www.zhihu.com/people/bopengbopeng)的[RWKV (100% RNN)语言模型](https://github.com/BlinkDL/RWKV-LM)驱动的类 ChatGPT， RNN 和 Transformer 的所有优点：高性能，快速运行，快速训练，节省显存。
+自动下载：
 
-模型的具体使用，还请关注[原仓库说明](https://github.com/BlinkDL/ChatRWKV)提交检测 →![GitHub last commit](https://img.shields.io/github/last-commit/BlinkDL/ChatRWKV?style=flat-square)
+- 无需设置，默认下载`ChatGLM-6B-INT4-QE`模型
+- 在`.env`文件中增加`chatglm_model = str`，其中 str 为字符串格式的 Hugging Face Hub 路径（用户名/仓库）。
+
+自动下载后转移模型到指定路径
+
+```python
+from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, AutoModel
+model_name = input("HF HUB 路径，例如 THUDM/chatglm-6b-int4-qe: ")
+model_path = input("本地存放路径，例如 ./path/modelname: ")
+#用 AutoModelForSeq2SeqLM.from_pretrained() 下载模型
+tokenizer = AutoTokenizer.from_pretrained(model_name,trust_remote_code=True,revision="main")
+model = AutoModelForSeq2SeqLM.from_pretrained(model_name,trust_remote_code=True,revision="main")
+#用 PreTrainedModel.save_pretrained() 保存模型到指定位置
+tokenizer.save_pretrained(model_path,trust_remote_code=True,revision="main")
+model.save_pretrained(model_path,trust_remote_code=True,revision="main")
+```
 
 手动下载：
 
-→[🤗 Hugging Face](https://huggingface.co/BlinkDL)，请根据自己的配置和需要，选择模型下载使用。
+- [清华云盘](https://cloud.tsinghua.edu.cn/d/fb9f16d6dc8f482596c2/)（仅模型文件，是 6B 完整模型，显存较小需要量化使用，暂未设置，需要自行在`chat.py`文件中修改）
+- [🤗 Hugging Face](https://huggingface.co/THUDM/chatglm-6b-int4)（完整文件），约 4.2 GB。
+
+#### 模型更新与其他使用
 
-个人建议，目前仅中文小说文本生成模型比较好用，8G 显存，推荐 3B 模型。
+模型的具体使用，还请关注 [原仓库说明](https://github.com/THUDM/ChatGLM-6B)，提交检测 →[![GitHub last commit](https://img.shields.io/github/last-commit/THUDM/ChatGLM-6B?style=flat-square)](https://github.com/THUDM/ChatGLM-6B)
 
-### 安装运行所需依赖
+### 运行所需依赖
 
 如果使用 pip 安装，实际已经自动安装了以下依赖，在此说明是为了方便检查
 
 1、模型所需的依赖
 
-ChatGLM，默认
+ChatGLM 推理
 
 ```bash
-pip install protobuf==3.20.0 transformers==4.26.1 icetk cpm_kernels
+pip install -U protobuf transformers>=4.23.1 cpm_kernels sentencepiece
 ```
 
-ChatRWKV，附加
+ChatGLM 微调
 
 ```bash
-pip install rwkv prompt_toolkit
+pip install -U rouge_chinese nltk jieba datasets
 ```
 
 2、`NoneBot`运行所需依赖
 
-安装这个插件，那必然是已经有了`NoneBot`项目，或者移步去[NoneBot2](https://github.com/nonebot/nonebot2)查看。由于还不会根据项目自动切换适配器，因此需要安装`nonebot-adapter-onebot`，以便调用`Onebotv11`进行通信。
+安装这个插件，那必然是已经有了`NoneBot`项目，或者移步去 [NoneBot2](https://github.com/nonebot/nonebot2) 查看。由于还不会根据项目自动切换适配器，因此需要安装`nonebot-adapter-onebot`，以便调用`Onebotv11`进行通信。
 
 ### 配置
 
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+在 nonebot2 项目的`.env`或`.env.prod`或`.env.dev`（根据实际选择）文件中添加下表中的配置。默认情况下，无需添加配置即可启用。
 
-|    配置项     | 必填 |     类型      |                                     默认值                                      |             说明             |
-| :-----------: | :--: | :-----------: | :-----------------------------------------------------------------------------: | :--------------------------: |
-|   chat_mode   |  否  |      str      |                                       cpu                                       |    运行模式，cuda 或 cpu     |
-| chatglm_model |  否  |      str      | "$User$/.cache/huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4/" | chatglm 模型及其配置文档路径 |
-|  chatglm_his  |  否  |      str      |                                "./data/history/"                                |       历史记录保存路径       |
-|  chatglm_cmd  |  否  | str/list[str] |                                      "hi"                                       |           对话命令           |
-|    chat_cd    |  否  |      int      |                                       30                                        |    冷却时间，避免高频调用    |
+| 配置项         | 必填 |   类型    | 默认值                                                                             |             说明             |
+| -------------- | :--: | :-------: | ---------------------------------------------------------------------------------- | :--------------------------: |
+| chat_mode      |  否  |    str    | cpu                                                                                |    运行模式，cuda 或 cpu     |
+| chatglm_model  |  否  |    str    | "./data/chatglm/model" | chatglm 模型及其配置文档路径 |
+| chatglm_path |  否  |    str    | "./data/chatglm/"                                                                  |       插件相关中间文件保存路径       |
+| chatglm_cmd    |  否  | list[str] | ["hi"]                                                                             |           对话命令           |
+| chat_cd        |  否  |    int    | 30                                                                                 |    冷却时间，避免高频调用    |
+| chatglm_memo | 否 | int | 5 | 保存对话轮数|
 
-## 使用
+> 如果要较好的使用，强烈建议将`chat_mode`设置为`cuda`。
+>
+> 正常聊天使用来说，30 秒冷却较为合适；复杂问题聊天，60 秒较为合适。建议根据实际测试进行调整。
 
-### 指令表
+### 附加文件
 
-|   指令   |  权限  | 需要@ |   范围    |          说明          |
-| :------: | :----: | :---: | :-------: | :--------------------: |
-|    hi    | 所有人 |  否   | 私聊/群聊 |    与 chatglm 对话     |
-| 清空记录 | 所有人 |  否   | 私聊/群聊 | 清空自己的对话历史记录 |
-| 导出记录 | 所有人 |  否   |   群聊    |   导出记录文件到群中   |
+（在基本功能完善后放出，在此之前，可以自建尝试）
 
-## ToDo
+### roles 格式
 
-- [x] 保存对话记录以实现多轮对话
-  - [x] 冷却时间
-  - [ ] 限制记忆轮数（~~在抄了，在抄了~~）
-- [ ] 配置角色功能，基本实现，正在物色适合适合 ChatGLM 的角色配置
-- [ ] 图片输出功能（~~在抄了，在抄了~~）
-- [ ] 其他中文文本生成模型
-  - [x] 尝试使用`ChatRWKV`
-- [ ] 管理员在线配置
-- [ ] @[Bot] 机器人 使用功能（调试阶段，我个人不太需要，不过后续加上吧）
+```Python
+{
+  "catgirl":"猫娘是一种拟人化的生物，其行为似猫但类人。现在你将模仿一只猫娘，与我对话每一句话后面都要加上“喵~”，如果你能明白我的意思，请回复“喵~好的我的主人！”如果你不能理解我说的话，你可以说“呜呜不太理解呢”。",
+}
+```
+
+> ChatGLM 可能发生记忆遗失，因此在进行角色扮演时，不要提问复杂内容。
+
+#### simple 格式
+
+示例如下
+
+```python
+{
+    r"你好[吗]?|hello": "您好，很高兴与您在此相遇，但是您想问什么呢？",
+    r"你是[谁？]?": "我是 ChatGLM，一个参数 62 亿的人工智能语言模型，由清华大学和智谱 AI 训练开源，代号 ChatGLM-6B",
+    r"你的(主人|master)是[谁？]?": f"[CQ:at,qq={superusers}]",
+}
+```
 
-如有其他功能需求，欢迎提 issues，当然如果您实现了某些功能或修复了问题，也非常欢迎您提 PR。
+## 使用
+
+### 指令表
 
-## 更新说明
+|   指令   |    权限    | 需要@ |   范围    | 说明                    |
+| :------: | :--------: | :---: | :-------: | ----------------------- |
+|    hi    |   所有人   |  否   | 私聊/群聊 | 与 chatglm 对话         |
+| 清空记录 |   所有人   |  否   | 私聊/群聊 | 清空自己的对话历史记录  |
+| 导出记录 |   所有人   |  否   |   群聊    | 导出记录文件到群中      |
+| 清理全部 | 超级管理员 |  否   |   私聊    | 手动处理`out of memory` |
 
-- 2023-03-22，更新说明文件，更新插件到 0.1.4，加入`ChatRWKV`生成中文小说文本，在配置使用`chatglm_mode="rwkv"`，并需修改模型路径（默认使用 cuda fp16 策略，如需修改，请自行更改`minirwkv.py`文件）
-- 2023-03-21，更新说明文件，更新插件到 0.1.3，默认使用`ChatGLM-6B-INT4`模型、CPU 推理，便于开箱即用；修复忘记设置包名导致的无法使用问题。
+## 参考与致谢
 
-## 致谢
+基础
 
 - [@A-kirami](https://github.com/A-kirami)，项目使用了 README[模板](https://github.com/A-kirami/nonebot-plugin-template)，有修改
 - [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B)，模型和使用方法来源，一切的核心
 - [nonebot2](https://github.com/nonebot/nonebot2)，一切的基础
-- [ChatRWKV](https://github.com/BlinkDL/ChatRWKV)，目前提供的中文小说续写功能来源于此
+
+功能
+
 - [nonebot-plugin-novelai](https://github.com/sena-nana/nonebot-plugin-novelai)，学习的对象，cd 使用来自于此
 - [nonebot-plugin-ChatGLM6B](https://github.com/QNLanYang/nonebot_plugin_ChatGLM6B)，与本项目相似，但本项目从中学习转图片、对话记忆。
+- [ChatGLM-6B API](https://github.com/imClumsyPanda/ChatGLM-6B-API)、[ChatGLM-webui](https://github.com/Akegarasu/ChatGLM-webui)
+
```

#### html2text {}

```diff
@@ -1,116 +1,162 @@
-                                   [nonebot]
- # nonebot-plugin-chatglm _â¨ NoneBot [ChatGLM-6B](https://github.com/THUDM/
-ChatGLM-6B) æ¯ææä»¶ â¨_ ![licese](https://img.shields.io/github/license/
-DaoMingze/zhukebot) ![Python](https://img.shields.io/badge/python-3.9+-blue) [!
- [pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://
- pdm.fming.dev) ![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm)
-## ä»ç» ä½¿ç¨[ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B)ä¸ºåç«¯ï¼
-[NoneBot2](https://github.com/nonebot/
-nonebot2)ä¸ºå¹³å°çæå¶ç®åçæ¬å°ä¸­æï¼æ±è¯­ï¼ AI chat æä»¶ã
-### ç¯å¢è¦æ± | éåç­çº§ | æä½æ¾å­ | | :------: | :------: | | FP16
-| 13GB | | INT8 | 10GB | | INT4 | 6GB | ä½¿ç¨ INT4 éååç[æ¨¡å](https:
-//huggingface.co/THUDM/chatglm-6b-int4)ãéè¦ 4.2 GB
-å·¦å³çå­å¨ç©ºé´ï¼æ¨¡åï¼ï¼NVIDIA æ¾å¡ï¼ä½¿ç¨ CUDAï¼ã6G
-åä»¥ä¸çæ¾å­ãç°å¨é»è®¤ä½¿ç¨ CPU
-æ¨çï¼æ¹ä¾¿å¼ç®±å³ç¨ï¼ä½éåº¦è¾æ¢ã > å®éå¯ä»¥ä½äº Python
-3.9ï¼ä½ none-adapter-onebot è¦æ± Python 3.8+ï¼ã ## å®è£ä¸æ´æ° ###
-è½¯ä»¶ç¯å¢ #### CUDA - Windowsï¼è§[CUDA å®æ¹ææ¡£|è±æ](https://
-docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html) -
-Linuxï¼è§[CUDA å®æ¹ææ¡£|è±æ](https://docs.nvidia.com/cuda/cuda-
-installation-guide-linux/index.html) #### PyTorch è§[PyTorch å®æ¹å¯¼å¼]
-(https://pytorch.org/get-started/locally/) ### æä»¶  ï¼ä¸ï¼ä½¿ç¨ nb-cli
-å®è£ä¸æ´æ° å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-chatglm
---upgrade ```   ï¼äºï¼ä½¿ç¨åç®¡çå¨å®è£ä¸æ´æ° 1ãå¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤ï¼  pip ```bash pip install nonebot-plugin-chatglm
-```   pdm ```bash pdm add nonebot-plugin-chatglm ```   poetry ```bash poetry
-add nonebot-plugin-chatglm ```   conda ```bash conda install nonebot-plugin-
-chatglm ```  2ãæå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶,
-å¨ `[tool.nonebot]` é¨åè¿½å åå¥ ```toml plugins =
-["nonebot_plugin_chatglm"] ```  ## éç½® ### ChatGLM æ¨¡å >
-æ¨¡åç®ä»ï¼ChatGLM-6B
-æ¯ä¸ä¸ªå¼æºçãæ¯æä¸­è±åè¯­çå¯¹è¯è¯­è¨æ¨¡åï¼åºäº[General
-Language Model (GLM) ](https://github.com/THUDM/GLM) æ¶æï¼å·æ 62
+Metadata-Version: 2.1 Name: nonebot-plugin-chatglm Version: 0.1.5 Summary:
+åºäºChatGLM-6BçNoneBot2æä»¶ License: MIT Author-email: dao_mingze
+163.com> Requires-Python: >=3.8 Project-URL: repository, https://github.com/
+DaoMingze/zhukebot/tree/main/zhukebot/plugins/chatglm Description-Content-Type:
+text/markdown
+                                  [nonebot]
+[NoneBotPluginText] # nonebot-plugin-chatglm _â¨ NoneBot [ChatGLM-6B](https://
+       github.com/THUDM/ChatGLM-6B) æ¯ææä»¶ â¨_ ![python](https://
+ img.shields.io/badge/python-3.8+-blue) [![Code Style](https://img.shields.io/
+  badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![pre-
+    commit.ci status](https://results.pre-commit.ci/badge/github/DaoMingze/
+  zhukebot/main.svg)](https://results.pre-commit.ci/latest/github/DaoMingze/
+   zhukebot/main) [![pdm-managed](https://img.shields.io/badge/pdm-managed-
+  blueviolet)](https://pdm.fming.dev) [![PyPI](https://img.shields.io/pypi/v/
+  nonebot_plugin_chatglm)](https://pypi.org/project/nonebot-plugin-chatglm) !
+  [PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm) !
+   [nonebot](https://img.shields.io/badge/nonebot-2-red) ![onebot](https://
+img.shields.io/badge/onebot-11-white) ![licese](https://img.shields.io/github/
+    license/DaoMingze/zhukebot) [![FOSSA Status](https://app.fossa.com/api/
+  projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://
+                            app.fossa.com/projects/
+           git%2Bgithub.com%2FDaoMingze%2Fzhukebot?ref=badge_shield)
+## ä»ç» ä½¿ç¨ [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) ä¸ºåç«¯ï¼
+[NoneBot2](https://github.com/nonebot/nonebot2)
+ä¸ºå¹³å°çæå¶ç®åçæ¬å°ä¸­æï¼æ±è¯­ï¼ AI chat æä»¶ã
+é¦æ¬¡å è½½ç­å¾æ¶é´è§ Hugging Face ä¸è½½éåº¦èå®ã ##
+[æ´æ°è¯´æ](changelog.md) å¦æå¶ä»åè½éæ±æçé®ï¼æ¬¢è¿æ
+issuesï¼å½ç¶å¦ææ¨å®ç°äºæäºåè½æä¿®å¤äºé®é¢ï¼ä¹éå¸¸æ¬¢è¿æ¨æ
+PRã ### å¾å - [ ] éå¶è®°å¿è½®æ°ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ]
+å¾çè¾åºåè½ï¼nonebot-plugin-
+htmlrenderï¼ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ] ç®¡çåå¨çº¿éç½® - [ ]
+å¢å åå¥è¯»åæ¬å°éç½®æä»¶ï¼jsonï¼ä»¥å®ç°éç½®çå¨çº¿ç­æ´æ°
+- [ ] @[Bot] æºå¨äºº
+ä½¿ç¨åè½ï¼è°è¯é¶æ®µï¼æä¸ªäººä¸å¤ªéè¦ï¼ä¸è¿åç»­å ä¸å§ï¼
+### åç»/åè½ - [x] å®åçé»è®¤éç½®ï¼å¼ç®±å³ç¨ã - [x]
+æ¨¡åèªå¨ä¸è½½å¹¶å­æ¾å°æå®ä½ç½®ï¼HuggingFace Hubæä¾ï¼ - [x]
+ä¿å­å¯¹è¯è®°å½ä»¥å®ç°å¤è½®å¯¹è¯ - [x]
+å·å´æ¶é´ï¼æ ¹æ®æµè¯ææï¼é»è®¤ 30 ç§ï¼ - [x]
+éç½®è§è²åè½ï¼åºæ¬å®ç° ### ç¯å¢è¦æ±
+| éåç­çº§ | æ¨ç | å¾®è° | ç­ç¥ | | -------------- | ---------- | ---
+         - | -------------------------: | | æ  | CPU | | .float() | |
+FP16ï¼æ éåï¼ | 13GB æ¾å­ | 14GB | .half().cuda() | | INT8 | 8GB æ¾å­
+    | 9GB | .half().quantize(8).cuda() | | INT4 | 6GB æ¾å­ | 7GB | .half
+  ().quantize(4).cuda() | | INT4 æ¨¡å | 5.2GB æ¾å­ | | .half().cuda() | |
+              INT4-QE æ¨¡å | 4.3GB æ¾å­ | | .half().cuda() |
+ç°å¨é»è®¤ä½¿ç¨ CPU æ¨çï¼æ¹ä¾¿å¼ç®±å³ç¨ï¼ä½éåº¦è¾æ¢ã
+ç¡¬ä»¶éæ±ä¸ï¼è®­ç»>å¾®è°>æ¨çï¼ä½æ¬æä»¶ä»èèæ¨çåºç¨åºæ¯ã
+> none-adapter-onebot è¦æ± Python 3.8+ ## å®è£ä¸æ´æ° ### è½¯ä»¶ç¯å¢
+æé¤å» Python å nonebot ä»¥å¤çè½¯ä»¶ç¯å¢ #### CUDA - Windowsï¼è§
+[CUDA å®æ¹ææ¡£ | è±æ](https://docs.nvidia.com/cuda/cuda-installation-
+guide-microsoft-windows/index.html) - Linuxï¼è§ [CUDA å®æ¹ææ¡£ | è±æ]
+(https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html) ####
+PyTorch è§ [PyTorch å®æ¹å¯¼å¼](https://pytorch.org/get-started/locally/
+) ### æä»¶  ï¼ä¸ï¼ä½¿ç¨ nb-cli å®è£ä¸æ´æ° å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡ï¼è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash
+nb plugin install nonebot-plugin-chatglm --upgrade ```
+ï¼äºï¼ä½¿ç¨åç®¡çå¨å®è£ä¸æ´æ° 1ãå¨ nonebot2
+é¡¹ç®çæä»¶ç®å½ä¸ï¼æå¼å½ä»¤è¡ï¼æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨ï¼è¾å¥ç¸åºçå®è£å½ä»¤ï¼
+pip ```bash pip install nonebot-plugin-chatglm ```   pdm ```bash pdm add
+nonebot-plugin-chatglm ```   poetry ```bash poetry add nonebot-plugin-chatglm
+```   conda ```bash conda install nonebot-plugin-chatglm ```  2ãæå¼
+nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶ï¼å¨ `[tool.nonebot]`
+é¨åè¿½å åå¥ ```toml plugins = ["nonebot_plugin_chatglm"] ```  ##
+éç½®ä¸ä¾èµ ### ChatGLM æ¨¡å > æ¨¡åç®ä»ï¼ChatGLM-6B
+æ¯ä¸ä¸ªå¼æºçãæ¯æä¸­è±åè¯­çå¯¹è¯è¯­è¨æ¨¡åï¼åºäº [General
+Language Model (GLM)](https://github.com/THUDM/GLM) æ¶æï¼å·æ 62
 äº¿åæ°ãç»åæ¨¡åéåææ¯ï¼ç¨æ·å¯ä»¥å¨æ¶è´¹çº§çæ¾å¡ä¸è¿è¡æ¬å°é¨ç½²ï¼INT4
 éåçº§å«ä¸æä½åªé 6GB æ¾å­ï¼ã ChatGLM-6B ä½¿ç¨äºå ChatGPT
 ç¸ä¼¼çææ¯ï¼éå¯¹ä¸­æé®ç­åå¯¹è¯è¿è¡äºä¼åãç»è¿çº¦ 1T
 æ è¯ç¬¦çä¸­è±åè¯­è®­ç»ï¼è¾ä»¥çç£å¾®è°ãåé¦èªå©ãäººç±»åé¦å¼ºåå­¦ä¹ ç­ææ¯çå æï¼62
 äº¿åæ°ç ChatGLM-6B å·²ç»è½çæç¸å½ç¬¦åäººç±»åå¥½çåç­ã
-é»è®¤ä½¿ç¨`HuggingFace
-Hub`å è½½ï¼å³å¦ææ²¡æè®¾ç½®è·¯å¾ï¼åä¼èªå¨ä¸è½½å°ç¨æ·ç®å½ä¸ç`.cache/
-huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4`ã -
-å¦ææ¯è¾å°æ¾å­ï¼< 10 Gï¼ä¸åªç¨èå¤©å¯¹è¯æ¨¡åï¼ChatGLM-6B-
-INT4ï¼[^1]åæ²¡ç¨å¿è¦ä¿®æ¹ã - å¦æä½¿ç¨ 6B
-å®æ´æ¨¡åï¼åå¯ä»¥èªè¡è®¾ç½®è·¯å¾ã
-æ¨¡åçå·ä½ä½¿ç¨ï¼è¿è¯·å³æ³¨[åä»åºè¯´æ](https://github.com/THUDM/
-ChatGLM-6B)æäº¤æ£æµ â![GitHub last commit](https://img.shields.io/github/
-last-commit/THUDM/ChatGLM-6B?style=flat-square) [^1]:
+#### éæ©æ¨¡å
+ChatGLM-6B ç³»åæ¨¡å | æ¨¡ååç§° | éåæåµ | æéå¤§å° | | ------
+--------------------------------------------------------------- | -------------
+  ---------------------- | -------: | | [ChatGLM-6B](https://huggingface.co/
+THUDM/chatglm-6b) | æ  | 13.73GB | | [ChatGLM-6B-INT4](https://huggingface.co/
+  THUDM/chatglm-6b-int4) | INT4: GLM Block | 4.06GB | | [ChatGLM-6B-INT4-QE]
+(https://huggingface.co/THUDM/chatglm-6b-int4-qe) | INT4: GLM Block, Embedding,
+                              LM Head | 3.13GB |
+- å¦ææ¯è¾å°æ¾å­ï¼< 10 Gï¼ä¸åªç¨èå¤©å¯¹è¯æ¨¡åï¼ChatGLM-6B-
+INT4-QEï¼[^1] åæ²¡ç¨å¿è¦ä¿®æ¹ã - å¦æä½¿ç¨ 6B
+å®æ´æ¨¡åï¼åå¯ä»¥èªè¡è®¾ç½®è·¯å¾ã [^1]:
 å¨å¶ä»ä½ç½®éç½®éååç INT4
-æ¨¡åï¼åçä¸äºç¼è¯éè¯¯ï¼ææ¶~~æå¾~~æ²¡æè½åè§£å³ã
-æå¨ä¸è½½ï¼ â[æ¸åäºç](https://cloud.tsinghua.edu.cn/d/
+æ¨¡åï¼åçä¸äºç¼è¯éè¯¯ï¼ææ¶~~æå¾~~æ²¡æè½åè§£å³ã ####
+ä¸è½½æ¨¡å é»è®¤ä½¿ç¨`HuggingFace
+Hub`å è½½ï¼å³å¦ææ²¡æè®¾ç½®è·¯å¾ï¼åä¼èªå¨ä¸è½½å°ç¨æ·ç®å½ä¸ç`.cache/
+huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4-
+qe`ï¼å¯ä»¥éè¿ä¸é¢çä»£ç è½¬ç§»æ¨¡åã èªå¨ä¸è½½ï¼ -
+æ éè®¾ç½®ï¼é»è®¤ä¸è½½`ChatGLM-6B-INT4-QE`æ¨¡å -
+å¨`.env`æä»¶ä¸­å¢å `chatglm_model = str`ï¼å¶ä¸­ str
+ä¸ºå­ç¬¦ä¸²æ ¼å¼ç Hugging Face Hub è·¯å¾ï¼ç¨æ·å/ä»åºï¼ã
+èªå¨ä¸è½½åè½¬ç§»æ¨¡åå°æå®è·¯å¾ ```python from transformers import
+AutoTokenizer, AutoModelForSeq2SeqLM, AutoModel model_name = input("HF HUB
+è·¯å¾ï¼ä¾å¦ THUDM/chatglm-6b-int4-qe: ") model_path = input
+("æ¬å°å­æ¾è·¯å¾ï¼ä¾å¦ ./path/modelname: ") #ç¨
+AutoModelForSeq2SeqLM.from_pretrained() ä¸è½½æ¨¡å tokenizer =
+AutoTokenizer.from_pretrained
+(model_name,trust_remote_code=True,revision="main") model =
+AutoModelForSeq2SeqLM.from_pretrained
+(model_name,trust_remote_code=True,revision="main") #ç¨
+PreTrainedModel.save_pretrained() ä¿å­æ¨¡åå°æå®ä½ç½®
+tokenizer.save_pretrained(model_path,trust_remote_code=True,revision="main")
+model.save_pretrained(model_path,trust_remote_code=True,revision="main") ```
+æå¨ä¸è½½ï¼ - [æ¸åäºç](https://cloud.tsinghua.edu.cn/d/
 fb9f16d6dc8f482596c2/)ï¼ä»æ¨¡åæä»¶ï¼æ¯ 6B
 å®æ´æ¨¡åï¼æ¾å­è¾å°éè¦éåä½¿ç¨ï¼ææªè®¾ç½®ï¼éè¦èªè¡å¨`chat.py`æä»¶ä¸­ä¿®æ¹ï¼
-â[ð¤ Hugging Face](https://huggingface.co/THUDM/chatglm-6b-
-int4)ï¼å®æ´æä»¶ï¼ï¼çº¦ 4.2 GBã ### ChatRWKV æ¨¡å >
-æ¨¡åç®ä»ï¼ChatRWKV is like ChatGPT but powered by my RWKV (100% RNN)
-language model, which is the only RNN (as of now) that can match transformers
-in quality and scaling, while being faster and saves VRAM. > > ChatRWKV
-æ¯ä¸ä¸ªç±[@PENG Bo](https://www.zhihu.com/people/bopengbopeng)ç[RWKV (100%
-RNN)è¯­è¨æ¨¡å](https://github.com/BlinkDL/RWKV-LM)é©±å¨çç±» ChatGPTï¼
-RNN å Transformer
-çææä¼ç¹ï¼é«æ§è½ï¼å¿«éè¿è¡ï¼å¿«éè®­ç»ï¼èçæ¾å­ã
-æ¨¡åçå·ä½ä½¿ç¨ï¼è¿è¯·å³æ³¨[åä»åºè¯´æ](https://github.com/
-BlinkDL/ChatRWKV)æäº¤æ£æµ â![GitHub last commit](https://img.shields.io/
-github/last-commit/BlinkDL/ChatRWKV?style=flat-square) æå¨ä¸è½½ï¼ â[ð¤
-Hugging Face](https://huggingface.co/
-BlinkDL)ï¼è¯·æ ¹æ®èªå·±çéç½®åéè¦ï¼éæ©æ¨¡åä¸è½½ä½¿ç¨ã
-ä¸ªäººå»ºè®®ï¼ç®åä»ä¸­æå°è¯´ææ¬çææ¨¡åæ¯è¾å¥½ç¨ï¼8G
-æ¾å­ï¼æ¨è 3B æ¨¡åã ### å®è£è¿è¡æéä¾èµ å¦æä½¿ç¨ pip
+- [ð¤ Hugging Face](https://huggingface.co/THUDM/chatglm-6b-
+int4)ï¼å®æ´æä»¶ï¼ï¼çº¦ 4.2 GBã #### æ¨¡åæ´æ°ä¸å¶ä»ä½¿ç¨
+æ¨¡åçå·ä½ä½¿ç¨ï¼è¿è¯·å³æ³¨ [åä»åºè¯´æ](https://github.com/
+THUDM/ChatGLM-6B)ï¼æäº¤æ£æµ â[![GitHub last commit](https://
+img.shields.io/github/last-commit/THUDM/ChatGLM-6B?style=flat-square)](https://
+github.com/THUDM/ChatGLM-6B) ### è¿è¡æéä¾èµ å¦æä½¿ç¨ pip
 å®è£ï¼å®éå·²ç»èªå¨å®è£äºä»¥ä¸ä¾èµï¼å¨æ­¤è¯´ææ¯ä¸ºäºæ¹ä¾¿æ£æ¥
-1ãæ¨¡åæéçä¾èµ ChatGLMï¼é»è®¤ ```bash pip install protobuf==3.20.0
-transformers==4.26.1 icetk cpm_kernels ``` ChatRWKVï¼éå  ```bash pip
-install rwkv prompt_toolkit ``` 2ã`NoneBot`è¿è¡æéä¾èµ
+1ãæ¨¡åæéçä¾èµ ChatGLM æ¨ç ```bash pip install -U protobuf
+transformers>=4.23.1 cpm_kernels sentencepiece ``` ChatGLM å¾®è° ```bash pip
+install -U rouge_chinese nltk jieba datasets ```
+2ã`NoneBot`è¿è¡æéä¾èµ
 å®è£è¿ä¸ªæä»¶ï¼é£å¿ç¶æ¯å·²ç»æäº`NoneBot`é¡¹ç®ï¼æèç§»æ­¥å»
-[NoneBot2](https://github.com/nonebot/
-nonebot2)æ¥çãç±äºè¿ä¸ä¼æ ¹æ®é¡¹ç®èªå¨åæ¢ééå¨ï¼å æ­¤éè¦å®è£`nonebot-
+[NoneBot2](https://github.com/nonebot/nonebot2)
+æ¥çãç±äºè¿ä¸ä¼æ ¹æ®é¡¹ç®èªå¨åæ¢ééå¨ï¼å æ­¤éè¦å®è£`nonebot-
 adapter-onebot`ï¼ä»¥ä¾¿è°ç¨`Onebotv11`è¿è¡éä¿¡ã ### éç½® å¨
-nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ |
-å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | | :-----------: | :--: | :-----------: |
-:-----------------------------------------------------------------------------:
-| :--------------------------: | | chat_mode | å¦ | str | cpu |
-è¿è¡æ¨¡å¼ï¼cuda æ cpu | | chatglm_model | å¦ | str | "$User$/.cache/
-huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4/" | chatglm
-æ¨¡ååå¶éç½®ææ¡£è·¯å¾ | | chatglm_his | å¦ | str | "./data/history/
-" | åå²è®°å½ä¿å­è·¯å¾ | | chatglm_cmd | å¦ | str/list[str] | "hi" |
-å¯¹è¯å½ä»¤ | | chat_cd | å¦ | int | 30 | å·å´æ¶é´ï¼é¿åé«é¢è°ç¨ |
-## ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :----
---: | :----: | :---: | :-------: | :--------------------: | | hi | ææäºº |
-å¦ | ç§è/ç¾¤è | ä¸ chatglm å¯¹è¯ | | æ¸ç©ºè®°å½ | ææäºº | å¦ |
-ç§è/ç¾¤è | æ¸ç©ºèªå·±çå¯¹è¯åå²è®°å½ | | å¯¼åºè®°å½ | ææäºº
-| å¦ | ç¾¤è | å¯¼åºè®°å½æä»¶å°ç¾¤ä¸­ | ## ToDo - [x]
-ä¿å­å¯¹è¯è®°å½ä»¥å®ç°å¤è½®å¯¹è¯ - [x] å·å´æ¶é´ - [ ]
-éå¶è®°å¿è½®æ°ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ]
-éç½®è§è²åè½ï¼åºæ¬å®ç°ï¼æ­£å¨ç©è²éåéå ChatGLM
-çè§è²éç½® - [ ] å¾çè¾åºåè½ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ]
-å¶ä»ä¸­æææ¬çææ¨¡å - [x] å°è¯ä½¿ç¨`ChatRWKV` - [ ]
-ç®¡çåå¨çº¿éç½® - [ ] @[Bot] æºå¨äºº
-ä½¿ç¨åè½ï¼è°è¯é¶æ®µï¼æä¸ªäººä¸å¤ªéè¦ï¼ä¸è¿åç»­å ä¸å§ï¼
-å¦æå¶ä»åè½éæ±ï¼æ¬¢è¿æ
-issuesï¼å½ç¶å¦ææ¨å®ç°äºæäºåè½æä¿®å¤äºé®é¢ï¼ä¹éå¸¸æ¬¢è¿æ¨æ
-PRã ## æ´æ°è¯´æ - 2023-03-22ï¼æ´æ°è¯´ææä»¶ï¼æ´æ°æä»¶å°
-0.1.4ï¼å å¥`ChatRWKV`çæä¸­æå°è¯´ææ¬ï¼å¨éç½®ä½¿ç¨`chatglm_mode="rwkv"`ï¼å¹¶éä¿®æ¹æ¨¡åè·¯å¾ï¼é»è®¤ä½¿ç¨
-cuda fp16 ç­ç¥ï¼å¦éä¿®æ¹ï¼è¯·èªè¡æ´æ¹`minirwkv.py`æä»¶ï¼ - 2023-
-03-21ï¼æ´æ°è¯´ææä»¶ï¼æ´æ°æä»¶å° 0.1.3ï¼é»è®¤ä½¿ç¨`ChatGLM-6B-
-INT4`æ¨¡åãCPU
-æ¨çï¼ä¾¿äºå¼ç®±å³ç¨ï¼ä¿®å¤å¿è®°è®¾ç½®ååå¯¼è´çæ æ³ä½¿ç¨é®é¢ã
-## è´è°¢ - [@A-kirami](https://github.com/A-kirami)ï¼é¡¹ç®ä½¿ç¨äº README
-[æ¨¡æ¿](https://github.com/A-kirami/nonebot-plugin-template)ï¼æä¿®æ¹ -
-[ChatGLM-6B](https://github.com/THUDM/ChatGLM-
-6B)ï¼æ¨¡ååä½¿ç¨æ¹æ³æ¥æºï¼ä¸åçæ ¸å¿ - [nonebot2](https://
-github.com/nonebot/nonebot2)ï¼ä¸åçåºç¡ - [ChatRWKV](https://github.com/
-BlinkDL/ChatRWKV)ï¼ç®åæä¾çä¸­æå°è¯´ç»­ååè½æ¥æºäºæ­¤ -
-[nonebot-plugin-novelai](https://github.com/sena-nana/nonebot-plugin-
+nonebot2
+é¡¹ç®ç`.env`æ`.env.prod`æ`.env.dev`ï¼æ ¹æ®å®ééæ©ï¼æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®ãé»è®¤æåµä¸ï¼æ éæ·»å éç½®å³å¯å¯ç¨ã
+| éç½®é¡¹ | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | | -------------- | :--: |
+:-------: | -------------------------------------------------------------------
+--------------- | :--------------------------: | | chat_mode | å¦ | str | cpu
+| è¿è¡æ¨¡å¼ï¼cuda æ cpu | | chatglm_model | å¦ | str | "./data/chatglm/
+model" | chatglm æ¨¡ååå¶éç½®ææ¡£è·¯å¾ | | chatglm_path | å¦ | str |
+"./data/chatglm/" | æä»¶ç¸å³ä¸­é´æä»¶ä¿å­è·¯å¾ | | chatglm_cmd | å¦
+| list[str] | ["hi"] | å¯¹è¯å½ä»¤ | | chat_cd | å¦ | int | 30 |
+å·å´æ¶é´ï¼é¿åé«é¢è°ç¨ | | chatglm_memo | å¦ | int | 5 |
+ä¿å­å¯¹è¯è½®æ°| >
+å¦æè¦è¾å¥½çä½¿ç¨ï¼å¼ºçå»ºè®®å°`chat_mode`è®¾ç½®ä¸º`cuda`ã > >
+æ­£å¸¸èå¤©ä½¿ç¨æ¥è¯´ï¼30 ç§å·å´è¾ä¸ºåéï¼å¤æé®é¢èå¤©ï¼60
+ç§è¾ä¸ºåéãå»ºè®®æ ¹æ®å®éæµè¯è¿è¡è°æ´ã ### éå æä»¶
+ï¼å¨åºæ¬åè½å®ååæ¾åºï¼å¨æ­¤ä¹åï¼å¯ä»¥èªå»ºå°è¯ï¼ ###
+roles æ ¼å¼ ```Python { "catgirl":
+"ç«å¨æ¯ä¸ç§æäººåççç©ï¼å¶è¡ä¸ºä¼¼ç«ä½ç±»äººãç°å¨ä½ å°æ¨¡ä»¿ä¸åªç«å¨ï¼ä¸æå¯¹è¯æ¯ä¸å¥è¯åé¢é½è¦å ä¸âåµ~âï¼å¦æä½ è½æç½æçææï¼è¯·åå¤âåµ~å¥½çæçä¸»äººï¼âå¦æä½ ä¸è½çè§£æè¯´çè¯ï¼ä½ å¯ä»¥è¯´âååä¸å¤ªçè§£å¢âã",
+} ``` > ChatGLM
+å¯è½åçè®°å¿éå¤±ï¼å æ­¤å¨è¿è¡è§è²æ®æ¼æ¶ï¼ä¸è¦æé®å¤æåå®¹ã
+#### simple æ ¼å¼ ç¤ºä¾å¦ä¸ ```python { r"ä½ å¥½[å]?|hello":
+"æ¨å¥½ï¼å¾é«å´ä¸æ¨å¨æ­¤ç¸éï¼ä½æ¯æ¨æ³é®ä»ä¹å¢ï¼", r"ä½ æ¯
+[è°ï¼]?": "ææ¯ ChatGLMï¼ä¸ä¸ªåæ° 62
+äº¿çäººå·¥æºè½è¯­è¨æ¨¡åï¼ç±æ¸åå¤§å­¦åæºè°± AI
+è®­ç»å¼æºï¼ä»£å· ChatGLM-6B", r"ä½ ç(ä¸»äºº|master)æ¯[è°ï¼]?": f"[CQ:
+at,qq={superusers}]", } ``` ## ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@
+| èå´ | è¯´æ | | :------: | :--------: | :---: | :-------: | -------------
+---------- | | hi | ææäºº | å¦ | ç§è/ç¾¤è | ä¸ chatglm å¯¹è¯ | |
+æ¸ç©ºè®°å½ | ææäºº | å¦ | ç§è/ç¾¤è |
+æ¸ç©ºèªå·±çå¯¹è¯åå²è®°å½ | | å¯¼åºè®°å½ | ææäºº | å¦ | ç¾¤è |
+å¯¼åºè®°å½æä»¶å°ç¾¤ä¸­ | | æ¸çå¨é¨ | è¶çº§ç®¡çå | å¦ | ç§è |
+æå¨å¤ç`out of memory` | ## åèä¸è´è°¢ åºç¡ - [@A-kirami](https://
+github.com/A-kirami)ï¼é¡¹ç®ä½¿ç¨äº README[æ¨¡æ¿](https://github.com/A-
+kirami/nonebot-plugin-template)ï¼æä¿®æ¹ - [ChatGLM-6B](https://github.com/
+THUDM/ChatGLM-6B)ï¼æ¨¡ååä½¿ç¨æ¹æ³æ¥æºï¼ä¸åçæ ¸å¿ - [nonebot2]
+(https://github.com/nonebot/nonebot2)ï¼ä¸åçåºç¡ åè½ - [nonebot-
+plugin-novelai](https://github.com/sena-nana/nonebot-plugin-
 novelai)ï¼å­¦ä¹ çå¯¹è±¡ï¼cd ä½¿ç¨æ¥èªäºæ­¤ - [nonebot-plugin-ChatGLM6B]
 (https://github.com/QNLanYang/
 nonebot_plugin_ChatGLM6B)ï¼ä¸æ¬é¡¹ç®ç¸ä¼¼ï¼ä½æ¬é¡¹ç®ä»ä¸­å­¦ä¹ è½¬å¾çãå¯¹è¯è®°å¿ã
+- [ChatGLM-6B API](https://github.com/imClumsyPanda/ChatGLM-6B-API)ã[ChatGLM-
+webui](https://github.com/Akegarasu/ChatGLM-webui)
```

### Comparing `nonebot-plugin-chatglm-0.1.4/pyproject.toml` & `nonebot-plugin-chatglm-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 [tool.pdm.build]
 includes = [
     "nonebot_plugin_chatglm",
 ]
 
 [project]
 name = "nonebot-plugin-chatglm"
-version = "0.1.4"
+version = "0.1.5"
 description = "基于ChatGLM-6B的NoneBot2插件"
 authors = [
     { name = "dao_mingze", email = "dao_mingze@163.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dependencies = [
-    "protobuf==3.20.0",
-    "transformers>=4.26.1",
+    "protobuf>=3.20.0",
+    "transformers>=4.27.1",
     "icetk>=0.0.4",
     "cpm-kernels>=1.0.11",
     "nonebot-adapter-onebot>=2.1.0",
     "nonebot2>=2.0.0rc3",
 ]
 
 [project.license]
```

### Comparing `nonebot-plugin-chatglm-0.1.4/PKG-INFO` & `nonebot-plugin-chatglm-0.1.5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,107 @@
-Metadata-Version: 2.1
-Name: nonebot-plugin-chatglm
-Version: 0.1.4
-Summary: 基于ChatGLM-6B的NoneBot2插件
-License: MIT
-Author-email: dao_mingze <dao_mingze@163.com>
-Requires-Python: >=3.8
-Project-URL: repository, https://github.com/DaoMingze/zhukebot/tree/main/zhukebot/plugins/chatglm
-Description-Content-Type: text/markdown
-
-<p align="center">
-  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>
-</p>
-
 <div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://ghproxy.com/https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="200" height="200" alt="nonebot"></a>
+<br/><img src="https://ghproxy.com/https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 
 # nonebot-plugin-chatglm
 
 _✨ NoneBot [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) 支持插件 ✨_
 
-![licese](https://img.shields.io/github/license/DaoMingze/zhukebot)
-![Python](https://img.shields.io/badge/python-3.9+-blue)
+![python](https://img.shields.io/badge/python-3.8+-blue)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/DaoMingze/zhukebot/main.svg)](https://results.pre-commit.ci/latest/github/DaoMingze/zhukebot/main)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
-![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm)
+[![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm)](https://pypi.org/project/nonebot-plugin-chatglm)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm)
+![nonebot](https://img.shields.io/badge/nonebot-2-red)
+![onebot](https://img.shields.io/badge/onebot-11-white)
+![licese](https://img.shields.io/github/license/DaoMingze/zhukebot)
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot?ref=badge_shield)
 
 </div>
 
 ## 介绍
 
-使用[ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B)为后端，[NoneBot2](https://github.com/nonebot/nonebot2)为平台的极其简单的本地中文（汉语） AI chat 插件。
+使用 [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) 为后端，[NoneBot2](https://github.com/nonebot/nonebot2) 为平台的极其简单的本地中文（汉语） AI chat 插件。
+
+首次加载等待时间视 Hugging Face 下载速度而定。
+
+## [更新说明](changelog.md)
+
+如有其他功能需求或疑问，欢迎提 issues，当然如果您实现了某些功能或修复了问题，也非常欢迎您提 PR。
+
+### 待办
+
+- [ ] 限制记忆轮数（~~在抄了，在抄了~~）
+- [ ] 图片输出功能（nonebot-plugin-htmlrender）（~~在抄了，在抄了~~）
+- [ ] 管理员在线配置
+  - [ ] 增加写入读取本地配置文件（json）以实现配置的在线热更新
+- [ ] @[Bot] 机器人 使用功能（调试阶段，我个人不太需要，不过后续加上吧）
+
+### 办结/功能
+
+- [x] 完善的默认配置，开箱即用。
+- [x] 模型自动下载并存放到指定位置（HuggingFace Hub提供）
+- [x] 保存对话记录以实现多轮对话
+- [x] 冷却时间（根据测试效果，默认 30 秒）
+- [x] 配置角色功能，基本实现
 
 ### 环境要求
 
-| 量化等级 | 最低显存 |
-| :------: | :------: |
-|   FP16   |   13GB   |
-|   INT8   |   10GB   |
-|   INT4   |   6GB    |
+<div align="center">
+
+| 量化等级       | 推理       | 微调 |                       策略 |
+| -------------- | ---------- | ---- | -------------------------: |
+| 无             | CPU        |      |                   .float() |
+| FP16（无量化） | 13GB 显存  | 14GB |             .half().cuda() |
+| INT8           | 8GB 显存   | 9GB  | .half().quantize(8).cuda() |
+| INT4           | 6GB 显存   | 7GB  | .half().quantize(4).cuda() |
+| INT4 模型      | 5.2GB 显存 |      |             .half().cuda() |
+| INT4-QE 模型   | 4.3GB 显存 |      |             .half().cuda() |
+
+</div>
+
+现在默认使用 CPU 推理，方便开箱即用，但速度较慢。
 
-使用 INT4 量化后的[模型](https://huggingface.co/THUDM/chatglm-6b-int4)。需要 4.2 GB 左右的存储空间（模型），NVIDIA 显卡（使用 CUDA）、6G 及以上的显存。现在默认使用 CPU 推理，方便开箱即用，但速度较慢。
+硬件需求上：训练>微调>推理，但本插件仅考虑推理应用场景。
 
-> 实际可以低于 Python 3.9（但 none-adapter-onebot 要求 Python 3.8+）。
+> none-adapter-onebot 要求 Python 3.8+
 
 ## 安装与更新
 
 ### 软件环境
 
+指除去 Python 和 nonebot 以外的软件环境
+
 #### CUDA
 
-- Windows：见[CUDA 官方文档|英文](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html)
-- Linux：见[CUDA 官方文档|英文](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html)
+- Windows：见 [CUDA 官方文档 | 英文](https://docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html)
+- Linux：见 [CUDA 官方文档 | 英文](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html)
 
 #### PyTorch
 
-见[PyTorch 官方导引](https://pytorch.org/get-started/locally/)
+见 [PyTorch 官方导引](https://pytorch.org/get-started/locally/)
 
 ### 插件
 
 <details>
 <summary><b>（一）使用 nb-cli 安装与更新</b></summary>
 
-在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
+在 nonebot2 项目的根目录下打开命令行，输入以下指令即可安装
 
 ```bash
 nb plugin install nonebot-plugin-chatglm --upgrade
 ```
 
 </details>
 
 <details>
 
 <summary><b>（二）使用包管理器安装与更新</b></summary>
-1、在 nonebot2 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令：
+1、在 nonebot2 项目的插件目录下，打开命令行，根据你使用的包管理器，输入相应的安装命令：
 <details>
 <summary>pip</summary>
 
 ```bash
 pip install nonebot-plugin-chatglm
 ```
 
@@ -100,122 +127,161 @@
 
 ```bash
 conda install nonebot-plugin-chatglm
 ```
 
 </details>
 
-2、打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分追加写入
+2、打开 nonebot2 项目根目录下的 `pyproject.toml` 文件，在 `[tool.nonebot]` 部分追加写入
 
 ```toml
 plugins = ["nonebot_plugin_chatglm"]
 ```
 
 </details>
 
-## 配置
+## 配置与依赖
 
 ### ChatGLM 模型
 
-> 模型简介：ChatGLM-6B 是一个开源的、支持中英双语的对话语言模型，基于[General Language Model (GLM) ](https://github.com/THUDM/GLM) 架构，具有 62 亿参数。结合模型量化技术，用户可以在消费级的显卡上进行本地部署（INT4 量化级别下最低只需 6GB 显存）。 ChatGLM-6B 使用了和 ChatGPT 相似的技术，针对中文问答和对话进行了优化。经过约 1T 标识符的中英双语训练，辅以监督微调、反馈自助、人类反馈强化学习等技术的加持，62 亿参数的 ChatGLM-6B 已经能生成相当符合人类偏好的回答。
+> 模型简介：ChatGLM-6B 是一个开源的、支持中英双语的对话语言模型，基于 [General Language Model (GLM)](https://github.com/THUDM/GLM) 架构，具有 62 亿参数。结合模型量化技术，用户可以在消费级的显卡上进行本地部署（INT4 量化级别下最低只需 6GB 显存）。 ChatGLM-6B 使用了和 ChatGPT 相似的技术，针对中文问答和对话进行了优化。经过约 1T 标识符的中英双语训练，辅以监督微调、反馈自助、人类反馈强化学习等技术的加持，62 亿参数的 ChatGLM-6B 已经能生成相当符合人类偏好的回答。
 
-默认使用`HuggingFace Hub`加载，即如果没有设置路径，则会自动下载到用户目录下的`.cache/huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4`。
+#### 选择模型
 
-- 如果是较小显存（< 10 G）且只用聊天对话模型（ChatGLM-6B-INT4）[^1]则没用必要修改。
-- 如果使用 6B 完整模型，则可以自行设置路径。
+<div align="center">
 
-模型的具体使用，还请关注[原仓库说明](https://github.com/THUDM/ChatGLM-6B)提交检测 →![GitHub last commit](https://img.shields.io/github/last-commit/THUDM/ChatGLM-6B?style=flat-square)
+ChatGLM-6B 系列模型
 
-[^1]: 在其他位置配置量化后的 INT4 模型，发生一些编译错误，暂时~~懒得~~没有能力解决。
+| 模型名称                                                              | 量化情况                            | 权重大小 |
+| --------------------------------------------------------------------- | ----------------------------------- | -------: |
+| [ChatGLM-6B](https://huggingface.co/THUDM/chatglm-6b)                 | 无                                  |  13.73GB |
+| [ChatGLM-6B-INT4](https://huggingface.co/THUDM/chatglm-6b-int4)       | INT4: GLM Block                     |   4.06GB |
+| [ChatGLM-6B-INT4-QE](https://huggingface.co/THUDM/chatglm-6b-int4-qe) | INT4: GLM Block, Embedding, LM Head |   3.13GB |
 
-手动下载：
+</div>
 
-→[清华云盘](https://cloud.tsinghua.edu.cn/d/fb9f16d6dc8f482596c2/)（仅模型文件，是 6B 完整模型，显存较小需要量化使用，暂未设置，需要自行在`chat.py`文件中修改）
+- 如果是较小显存（< 10 G）且只用聊天对话模型（ChatGLM-6B-INT4-QE）[^1] 则没用必要修改。
+- 如果使用 6B 完整模型，则可以自行设置路径。
 
-→[🤗 Hugging Face](https://huggingface.co/THUDM/chatglm-6b-int4)（完整文件），约 4.2 GB。
+[^1]: 在其他位置配置量化后的 INT4 模型，发生一些编译错误，暂时~~懒得~~没有能力解决。
 
-### ChatRWKV 模型
+#### 下载模型
 
-> 模型简介：ChatRWKV is like ChatGPT but powered by my RWKV (100% RNN) language model, which is the only RNN (as of now) that can match transformers in quality and scaling, while being faster and saves VRAM.
->
-> ChatRWKV 是一个由[@PENG Bo](https://www.zhihu.com/people/bopengbopeng)的[RWKV (100% RNN)语言模型](https://github.com/BlinkDL/RWKV-LM)驱动的类 ChatGPT， RNN 和 Transformer 的所有优点：高性能，快速运行，快速训练，节省显存。
+默认使用`HuggingFace Hub`加载，即如果没有设置路径，则会自动下载到用户目录下的`.cache/huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4-qe`，可以通过下面的代码转移模型。
+
+自动下载：
 
-模型的具体使用，还请关注[原仓库说明](https://github.com/BlinkDL/ChatRWKV)提交检测 →![GitHub last commit](https://img.shields.io/github/last-commit/BlinkDL/ChatRWKV?style=flat-square)
+- 无需设置，默认下载`ChatGLM-6B-INT4-QE`模型
+- 在`.env`文件中增加`chatglm_model = str`，其中 str 为字符串格式的 Hugging Face Hub 路径（用户名/仓库）。
+
+自动下载后转移模型到指定路径
+
+```python
+from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, AutoModel
+model_name = input("HF HUB 路径，例如 THUDM/chatglm-6b-int4-qe: ")
+model_path = input("本地存放路径，例如 ./path/modelname: ")
+#用 AutoModelForSeq2SeqLM.from_pretrained() 下载模型
+tokenizer = AutoTokenizer.from_pretrained(model_name,trust_remote_code=True,revision="main")
+model = AutoModelForSeq2SeqLM.from_pretrained(model_name,trust_remote_code=True,revision="main")
+#用 PreTrainedModel.save_pretrained() 保存模型到指定位置
+tokenizer.save_pretrained(model_path,trust_remote_code=True,revision="main")
+model.save_pretrained(model_path,trust_remote_code=True,revision="main")
+```
 
 手动下载：
 
-→[🤗 Hugging Face](https://huggingface.co/BlinkDL)，请根据自己的配置和需要，选择模型下载使用。
+- [清华云盘](https://cloud.tsinghua.edu.cn/d/fb9f16d6dc8f482596c2/)（仅模型文件，是 6B 完整模型，显存较小需要量化使用，暂未设置，需要自行在`chat.py`文件中修改）
+- [🤗 Hugging Face](https://huggingface.co/THUDM/chatglm-6b-int4)（完整文件），约 4.2 GB。
+
+#### 模型更新与其他使用
 
-个人建议，目前仅中文小说文本生成模型比较好用，8G 显存，推荐 3B 模型。
+模型的具体使用，还请关注 [原仓库说明](https://github.com/THUDM/ChatGLM-6B)，提交检测 →[![GitHub last commit](https://img.shields.io/github/last-commit/THUDM/ChatGLM-6B?style=flat-square)](https://github.com/THUDM/ChatGLM-6B)
 
-### 安装运行所需依赖
+### 运行所需依赖
 
 如果使用 pip 安装，实际已经自动安装了以下依赖，在此说明是为了方便检查
 
 1、模型所需的依赖
 
-ChatGLM，默认
+ChatGLM 推理
 
 ```bash
-pip install protobuf==3.20.0 transformers==4.26.1 icetk cpm_kernels
+pip install -U protobuf transformers>=4.23.1 cpm_kernels sentencepiece
 ```
 
-ChatRWKV，附加
+ChatGLM 微调
 
 ```bash
-pip install rwkv prompt_toolkit
+pip install -U rouge_chinese nltk jieba datasets
 ```
 
 2、`NoneBot`运行所需依赖
 
-安装这个插件，那必然是已经有了`NoneBot`项目，或者移步去[NoneBot2](https://github.com/nonebot/nonebot2)查看。由于还不会根据项目自动切换适配器，因此需要安装`nonebot-adapter-onebot`，以便调用`Onebotv11`进行通信。
+安装这个插件，那必然是已经有了`NoneBot`项目，或者移步去 [NoneBot2](https://github.com/nonebot/nonebot2) 查看。由于还不会根据项目自动切换适配器，因此需要安装`nonebot-adapter-onebot`，以便调用`Onebotv11`进行通信。
 
 ### 配置
 
-在 nonebot2 项目的`.env`文件中添加下表中的必填配置
+在 nonebot2 项目的`.env`或`.env.prod`或`.env.dev`（根据实际选择）文件中添加下表中的配置。默认情况下，无需添加配置即可启用。
 
-|    配置项     | 必填 |     类型      |                                     默认值                                      |             说明             |
-| :-----------: | :--: | :-----------: | :-----------------------------------------------------------------------------: | :--------------------------: |
-|   chat_mode   |  否  |      str      |                                       cpu                                       |    运行模式，cuda 或 cpu     |
-| chatglm_model |  否  |      str      | "$User$/.cache/huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4/" | chatglm 模型及其配置文档路径 |
-|  chatglm_his  |  否  |      str      |                                "./data/history/"                                |       历史记录保存路径       |
-|  chatglm_cmd  |  否  | str/list[str] |                                      "hi"                                       |           对话命令           |
-|    chat_cd    |  否  |      int      |                                       30                                        |    冷却时间，避免高频调用    |
+| 配置项         | 必填 |   类型    | 默认值                                                                             |             说明             |
+| -------------- | :--: | :-------: | ---------------------------------------------------------------------------------- | :--------------------------: |
+| chat_mode      |  否  |    str    | cpu                                                                                |    运行模式，cuda 或 cpu     |
+| chatglm_model  |  否  |    str    | "./data/chatglm/model" | chatglm 模型及其配置文档路径 |
+| chatglm_path |  否  |    str    | "./data/chatglm/"                                                                  |       插件相关中间文件保存路径       |
+| chatglm_cmd    |  否  | list[str] | ["hi"]                                                                             |           对话命令           |
+| chat_cd        |  否  |    int    | 30                                                                                 |    冷却时间，避免高频调用    |
+| chatglm_memo | 否 | int | 5 | 保存对话轮数|
 
-## 使用
+> 如果要较好的使用，强烈建议将`chat_mode`设置为`cuda`。
+>
+> 正常聊天使用来说，30 秒冷却较为合适；复杂问题聊天，60 秒较为合适。建议根据实际测试进行调整。
 
-### 指令表
+### 附加文件
 
-|   指令   |  权限  | 需要@ |   范围    |          说明          |
-| :------: | :----: | :---: | :-------: | :--------------------: |
-|    hi    | 所有人 |  否   | 私聊/群聊 |    与 chatglm 对话     |
-| 清空记录 | 所有人 |  否   | 私聊/群聊 | 清空自己的对话历史记录 |
-| 导出记录 | 所有人 |  否   |   群聊    |   导出记录文件到群中   |
+（在基本功能完善后放出，在此之前，可以自建尝试）
 
-## ToDo
+### roles 格式
 
-- [x] 保存对话记录以实现多轮对话
-  - [x] 冷却时间
-  - [ ] 限制记忆轮数（~~在抄了，在抄了~~）
-- [ ] 配置角色功能，基本实现，正在物色适合适合 ChatGLM 的角色配置
-- [ ] 图片输出功能（~~在抄了，在抄了~~）
-- [ ] 其他中文文本生成模型
-  - [x] 尝试使用`ChatRWKV`
-- [ ] 管理员在线配置
-- [ ] @[Bot] 机器人 使用功能（调试阶段，我个人不太需要，不过后续加上吧）
+```Python
+{
+  "catgirl":"猫娘是一种拟人化的生物，其行为似猫但类人。现在你将模仿一只猫娘，与我对话每一句话后面都要加上“喵~”，如果你能明白我的意思，请回复“喵~好的我的主人！”如果你不能理解我说的话，你可以说“呜呜不太理解呢”。",
+}
+```
+
+> ChatGLM 可能发生记忆遗失，因此在进行角色扮演时，不要提问复杂内容。
+
+#### simple 格式
+
+示例如下
+
+```python
+{
+    r"你好[吗]?|hello": "您好，很高兴与您在此相遇，但是您想问什么呢？",
+    r"你是[谁？]?": "我是 ChatGLM，一个参数 62 亿的人工智能语言模型，由清华大学和智谱 AI 训练开源，代号 ChatGLM-6B",
+    r"你的(主人|master)是[谁？]?": f"[CQ:at,qq={superusers}]",
+}
+```
 
-如有其他功能需求，欢迎提 issues，当然如果您实现了某些功能或修复了问题，也非常欢迎您提 PR。
+## 使用
+
+### 指令表
 
-## 更新说明
+|   指令   |    权限    | 需要@ |   范围    | 说明                    |
+| :------: | :--------: | :---: | :-------: | ----------------------- |
+|    hi    |   所有人   |  否   | 私聊/群聊 | 与 chatglm 对话         |
+| 清空记录 |   所有人   |  否   | 私聊/群聊 | 清空自己的对话历史记录  |
+| 导出记录 |   所有人   |  否   |   群聊    | 导出记录文件到群中      |
+| 清理全部 | 超级管理员 |  否   |   私聊    | 手动处理`out of memory` |
 
-- 2023-03-22，更新说明文件，更新插件到 0.1.4，加入`ChatRWKV`生成中文小说文本，在配置使用`chatglm_mode="rwkv"`，并需修改模型路径（默认使用 cuda fp16 策略，如需修改，请自行更改`minirwkv.py`文件）
-- 2023-03-21，更新说明文件，更新插件到 0.1.3，默认使用`ChatGLM-6B-INT4`模型、CPU 推理，便于开箱即用；修复忘记设置包名导致的无法使用问题。
+## 参考与致谢
 
-## 致谢
+基础
 
 - [@A-kirami](https://github.com/A-kirami)，项目使用了 README[模板](https://github.com/A-kirami/nonebot-plugin-template)，有修改
 - [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B)，模型和使用方法来源，一切的核心
 - [nonebot2](https://github.com/nonebot/nonebot2)，一切的基础
-- [ChatRWKV](https://github.com/BlinkDL/ChatRWKV)，目前提供的中文小说续写功能来源于此
+
+功能
+
 - [nonebot-plugin-novelai](https://github.com/sena-nana/nonebot-plugin-novelai)，学习的对象，cd 使用来自于此
 - [nonebot-plugin-ChatGLM6B](https://github.com/QNLanYang/nonebot_plugin_ChatGLM6B)，与本项目相似，但本项目从中学习转图片、对话记忆。
-
+- [ChatGLM-6B API](https://github.com/imClumsyPanda/ChatGLM-6B-API)、[ChatGLM-webui](https://github.com/Akegarasu/ChatGLM-webui)
```

#### html2text {}

```diff
@@ -1,121 +1,157 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-chatglm Version: 0.1.4 Summary:
-åºäºChatGLM-6BçNoneBot2æä»¶ License: MIT Author-email: dao_mingze
-163.com> Requires-Python: >=3.8 Project-URL: repository, https://github.com/
-DaoMingze/zhukebot/tree/main/zhukebot/plugins/chatglm Description-Content-Type:
-text/markdown
-                                   [nonebot]
- # nonebot-plugin-chatglm _â¨ NoneBot [ChatGLM-6B](https://github.com/THUDM/
-ChatGLM-6B) æ¯ææä»¶ â¨_ ![licese](https://img.shields.io/github/license/
-DaoMingze/zhukebot) ![Python](https://img.shields.io/badge/python-3.9+-blue) [!
- [pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://
- pdm.fming.dev) ![PyPI](https://img.shields.io/pypi/v/nonebot_plugin_chatglm)
-## ä»ç» ä½¿ç¨[ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B)ä¸ºåç«¯ï¼
-[NoneBot2](https://github.com/nonebot/
-nonebot2)ä¸ºå¹³å°çæå¶ç®åçæ¬å°ä¸­æï¼æ±è¯­ï¼ AI chat æä»¶ã
-### ç¯å¢è¦æ± | éåç­çº§ | æä½æ¾å­ | | :------: | :------: | | FP16
-| 13GB | | INT8 | 10GB | | INT4 | 6GB | ä½¿ç¨ INT4 éååç[æ¨¡å](https:
-//huggingface.co/THUDM/chatglm-6b-int4)ãéè¦ 4.2 GB
-å·¦å³çå­å¨ç©ºé´ï¼æ¨¡åï¼ï¼NVIDIA æ¾å¡ï¼ä½¿ç¨ CUDAï¼ã6G
-åä»¥ä¸çæ¾å­ãç°å¨é»è®¤ä½¿ç¨ CPU
-æ¨çï¼æ¹ä¾¿å¼ç®±å³ç¨ï¼ä½éåº¦è¾æ¢ã > å®éå¯ä»¥ä½äº Python
-3.9ï¼ä½ none-adapter-onebot è¦æ± Python 3.8+ï¼ã ## å®è£ä¸æ´æ° ###
-è½¯ä»¶ç¯å¢ #### CUDA - Windowsï¼è§[CUDA å®æ¹ææ¡£|è±æ](https://
-docs.nvidia.com/cuda/cuda-installation-guide-microsoft-windows/index.html) -
-Linuxï¼è§[CUDA å®æ¹ææ¡£|è±æ](https://docs.nvidia.com/cuda/cuda-
-installation-guide-linux/index.html) #### PyTorch è§[PyTorch å®æ¹å¯¼å¼]
-(https://pytorch.org/get-started/locally/) ### æä»¶  ï¼ä¸ï¼ä½¿ç¨ nb-cli
-å®è£ä¸æ´æ° å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-chatglm
---upgrade ```   ï¼äºï¼ä½¿ç¨åç®¡çå¨å®è£ä¸æ´æ° 1ãå¨ nonebot2
-é¡¹ç®çæä»¶ç®å½ä¸, æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨,
-è¾å¥ç¸åºçå®è£å½ä»¤ï¼  pip ```bash pip install nonebot-plugin-chatglm
-```   pdm ```bash pdm add nonebot-plugin-chatglm ```   poetry ```bash poetry
-add nonebot-plugin-chatglm ```   conda ```bash conda install nonebot-plugin-
-chatglm ```  2ãæå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶,
-å¨ `[tool.nonebot]` é¨åè¿½å åå¥ ```toml plugins =
-["nonebot_plugin_chatglm"] ```  ## éç½® ### ChatGLM æ¨¡å >
-æ¨¡åç®ä»ï¼ChatGLM-6B
-æ¯ä¸ä¸ªå¼æºçãæ¯æä¸­è±åè¯­çå¯¹è¯è¯­è¨æ¨¡åï¼åºäº[General
-Language Model (GLM) ](https://github.com/THUDM/GLM) æ¶æï¼å·æ 62
+                                  [nonebot]
+[NoneBotPluginText] # nonebot-plugin-chatglm _â¨ NoneBot [ChatGLM-6B](https://
+       github.com/THUDM/ChatGLM-6B) æ¯ææä»¶ â¨_ ![python](https://
+ img.shields.io/badge/python-3.8+-blue) [![Code Style](https://img.shields.io/
+  badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![pre-
+    commit.ci status](https://results.pre-commit.ci/badge/github/DaoMingze/
+  zhukebot/main.svg)](https://results.pre-commit.ci/latest/github/DaoMingze/
+   zhukebot/main) [![pdm-managed](https://img.shields.io/badge/pdm-managed-
+  blueviolet)](https://pdm.fming.dev) [![PyPI](https://img.shields.io/pypi/v/
+  nonebot_plugin_chatglm)](https://pypi.org/project/nonebot-plugin-chatglm) !
+  [PyPI - Downloads](https://img.shields.io/pypi/dm/nonebot-plugin-chatglm) !
+   [nonebot](https://img.shields.io/badge/nonebot-2-red) ![onebot](https://
+img.shields.io/badge/onebot-11-white) ![licese](https://img.shields.io/github/
+    license/DaoMingze/zhukebot) [![FOSSA Status](https://app.fossa.com/api/
+  projects/git%2Bgithub.com%2FDaoMingze%2Fzhukebot.svg?type=shield)](https://
+                            app.fossa.com/projects/
+           git%2Bgithub.com%2FDaoMingze%2Fzhukebot?ref=badge_shield)
+## ä»ç» ä½¿ç¨ [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B) ä¸ºåç«¯ï¼
+[NoneBot2](https://github.com/nonebot/nonebot2)
+ä¸ºå¹³å°çæå¶ç®åçæ¬å°ä¸­æï¼æ±è¯­ï¼ AI chat æä»¶ã
+é¦æ¬¡å è½½ç­å¾æ¶é´è§ Hugging Face ä¸è½½éåº¦èå®ã ##
+[æ´æ°è¯´æ](changelog.md) å¦æå¶ä»åè½éæ±æçé®ï¼æ¬¢è¿æ
+issuesï¼å½ç¶å¦ææ¨å®ç°äºæäºåè½æä¿®å¤äºé®é¢ï¼ä¹éå¸¸æ¬¢è¿æ¨æ
+PRã ### å¾å - [ ] éå¶è®°å¿è½®æ°ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ]
+å¾çè¾åºåè½ï¼nonebot-plugin-
+htmlrenderï¼ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ] ç®¡çåå¨çº¿éç½® - [ ]
+å¢å åå¥è¯»åæ¬å°éç½®æä»¶ï¼jsonï¼ä»¥å®ç°éç½®çå¨çº¿ç­æ´æ°
+- [ ] @[Bot] æºå¨äºº
+ä½¿ç¨åè½ï¼è°è¯é¶æ®µï¼æä¸ªäººä¸å¤ªéè¦ï¼ä¸è¿åç»­å ä¸å§ï¼
+### åç»/åè½ - [x] å®åçé»è®¤éç½®ï¼å¼ç®±å³ç¨ã - [x]
+æ¨¡åèªå¨ä¸è½½å¹¶å­æ¾å°æå®ä½ç½®ï¼HuggingFace Hubæä¾ï¼ - [x]
+ä¿å­å¯¹è¯è®°å½ä»¥å®ç°å¤è½®å¯¹è¯ - [x]
+å·å´æ¶é´ï¼æ ¹æ®æµè¯ææï¼é»è®¤ 30 ç§ï¼ - [x]
+éç½®è§è²åè½ï¼åºæ¬å®ç° ### ç¯å¢è¦æ±
+| éåç­çº§ | æ¨ç | å¾®è° | ç­ç¥ | | -------------- | ---------- | ---
+         - | -------------------------: | | æ  | CPU | | .float() | |
+FP16ï¼æ éåï¼ | 13GB æ¾å­ | 14GB | .half().cuda() | | INT8 | 8GB æ¾å­
+    | 9GB | .half().quantize(8).cuda() | | INT4 | 6GB æ¾å­ | 7GB | .half
+  ().quantize(4).cuda() | | INT4 æ¨¡å | 5.2GB æ¾å­ | | .half().cuda() | |
+              INT4-QE æ¨¡å | 4.3GB æ¾å­ | | .half().cuda() |
+ç°å¨é»è®¤ä½¿ç¨ CPU æ¨çï¼æ¹ä¾¿å¼ç®±å³ç¨ï¼ä½éåº¦è¾æ¢ã
+ç¡¬ä»¶éæ±ä¸ï¼è®­ç»>å¾®è°>æ¨çï¼ä½æ¬æä»¶ä»èèæ¨çåºç¨åºæ¯ã
+> none-adapter-onebot è¦æ± Python 3.8+ ## å®è£ä¸æ´æ° ### è½¯ä»¶ç¯å¢
+æé¤å» Python å nonebot ä»¥å¤çè½¯ä»¶ç¯å¢ #### CUDA - Windowsï¼è§
+[CUDA å®æ¹ææ¡£ | è±æ](https://docs.nvidia.com/cuda/cuda-installation-
+guide-microsoft-windows/index.html) - Linuxï¼è§ [CUDA å®æ¹ææ¡£ | è±æ]
+(https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html) ####
+PyTorch è§ [PyTorch å®æ¹å¯¼å¼](https://pytorch.org/get-started/locally/
+) ### æä»¶  ï¼ä¸ï¼ä½¿ç¨ nb-cli å®è£ä¸æ´æ° å¨ nonebot2
+é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡ï¼è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash
+nb plugin install nonebot-plugin-chatglm --upgrade ```
+ï¼äºï¼ä½¿ç¨åç®¡çå¨å®è£ä¸æ´æ° 1ãå¨ nonebot2
+é¡¹ç®çæä»¶ç®å½ä¸ï¼æå¼å½ä»¤è¡ï¼æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨ï¼è¾å¥ç¸åºçå®è£å½ä»¤ï¼
+pip ```bash pip install nonebot-plugin-chatglm ```   pdm ```bash pdm add
+nonebot-plugin-chatglm ```   poetry ```bash poetry add nonebot-plugin-chatglm
+```   conda ```bash conda install nonebot-plugin-chatglm ```  2ãæå¼
+nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶ï¼å¨ `[tool.nonebot]`
+é¨åè¿½å åå¥ ```toml plugins = ["nonebot_plugin_chatglm"] ```  ##
+éç½®ä¸ä¾èµ ### ChatGLM æ¨¡å > æ¨¡åç®ä»ï¼ChatGLM-6B
+æ¯ä¸ä¸ªå¼æºçãæ¯æä¸­è±åè¯­çå¯¹è¯è¯­è¨æ¨¡åï¼åºäº [General
+Language Model (GLM)](https://github.com/THUDM/GLM) æ¶æï¼å·æ 62
 äº¿åæ°ãç»åæ¨¡åéåææ¯ï¼ç¨æ·å¯ä»¥å¨æ¶è´¹çº§çæ¾å¡ä¸è¿è¡æ¬å°é¨ç½²ï¼INT4
 éåçº§å«ä¸æä½åªé 6GB æ¾å­ï¼ã ChatGLM-6B ä½¿ç¨äºå ChatGPT
 ç¸ä¼¼çææ¯ï¼éå¯¹ä¸­æé®ç­åå¯¹è¯è¿è¡äºä¼åãç»è¿çº¦ 1T
 æ è¯ç¬¦çä¸­è±åè¯­è®­ç»ï¼è¾ä»¥çç£å¾®è°ãåé¦èªå©ãäººç±»åé¦å¼ºåå­¦ä¹ ç­ææ¯çå æï¼62
 äº¿åæ°ç ChatGLM-6B å·²ç»è½çæç¸å½ç¬¦åäººç±»åå¥½çåç­ã
-é»è®¤ä½¿ç¨`HuggingFace
-Hub`å è½½ï¼å³å¦ææ²¡æè®¾ç½®è·¯å¾ï¼åä¼èªå¨ä¸è½½å°ç¨æ·ç®å½ä¸ç`.cache/
-huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4`ã -
-å¦ææ¯è¾å°æ¾å­ï¼< 10 Gï¼ä¸åªç¨èå¤©å¯¹è¯æ¨¡åï¼ChatGLM-6B-
-INT4ï¼[^1]åæ²¡ç¨å¿è¦ä¿®æ¹ã - å¦æä½¿ç¨ 6B
-å®æ´æ¨¡åï¼åå¯ä»¥èªè¡è®¾ç½®è·¯å¾ã
-æ¨¡åçå·ä½ä½¿ç¨ï¼è¿è¯·å³æ³¨[åä»åºè¯´æ](https://github.com/THUDM/
-ChatGLM-6B)æäº¤æ£æµ â![GitHub last commit](https://img.shields.io/github/
-last-commit/THUDM/ChatGLM-6B?style=flat-square) [^1]:
+#### éæ©æ¨¡å
+ChatGLM-6B ç³»åæ¨¡å | æ¨¡ååç§° | éåæåµ | æéå¤§å° | | ------
+--------------------------------------------------------------- | -------------
+  ---------------------- | -------: | | [ChatGLM-6B](https://huggingface.co/
+THUDM/chatglm-6b) | æ  | 13.73GB | | [ChatGLM-6B-INT4](https://huggingface.co/
+  THUDM/chatglm-6b-int4) | INT4: GLM Block | 4.06GB | | [ChatGLM-6B-INT4-QE]
+(https://huggingface.co/THUDM/chatglm-6b-int4-qe) | INT4: GLM Block, Embedding,
+                              LM Head | 3.13GB |
+- å¦ææ¯è¾å°æ¾å­ï¼< 10 Gï¼ä¸åªç¨èå¤©å¯¹è¯æ¨¡åï¼ChatGLM-6B-
+INT4-QEï¼[^1] åæ²¡ç¨å¿è¦ä¿®æ¹ã - å¦æä½¿ç¨ 6B
+å®æ´æ¨¡åï¼åå¯ä»¥èªè¡è®¾ç½®è·¯å¾ã [^1]:
 å¨å¶ä»ä½ç½®éç½®éååç INT4
-æ¨¡åï¼åçä¸äºç¼è¯éè¯¯ï¼ææ¶~~æå¾~~æ²¡æè½åè§£å³ã
-æå¨ä¸è½½ï¼ â[æ¸åäºç](https://cloud.tsinghua.edu.cn/d/
+æ¨¡åï¼åçä¸äºç¼è¯éè¯¯ï¼ææ¶~~æå¾~~æ²¡æè½åè§£å³ã ####
+ä¸è½½æ¨¡å é»è®¤ä½¿ç¨`HuggingFace
+Hub`å è½½ï¼å³å¦ææ²¡æè®¾ç½®è·¯å¾ï¼åä¼èªå¨ä¸è½½å°ç¨æ·ç®å½ä¸ç`.cache/
+huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4-
+qe`ï¼å¯ä»¥éè¿ä¸é¢çä»£ç è½¬ç§»æ¨¡åã èªå¨ä¸è½½ï¼ -
+æ éè®¾ç½®ï¼é»è®¤ä¸è½½`ChatGLM-6B-INT4-QE`æ¨¡å -
+å¨`.env`æä»¶ä¸­å¢å `chatglm_model = str`ï¼å¶ä¸­ str
+ä¸ºå­ç¬¦ä¸²æ ¼å¼ç Hugging Face Hub è·¯å¾ï¼ç¨æ·å/ä»åºï¼ã
+èªå¨ä¸è½½åè½¬ç§»æ¨¡åå°æå®è·¯å¾ ```python from transformers import
+AutoTokenizer, AutoModelForSeq2SeqLM, AutoModel model_name = input("HF HUB
+è·¯å¾ï¼ä¾å¦ THUDM/chatglm-6b-int4-qe: ") model_path = input
+("æ¬å°å­æ¾è·¯å¾ï¼ä¾å¦ ./path/modelname: ") #ç¨
+AutoModelForSeq2SeqLM.from_pretrained() ä¸è½½æ¨¡å tokenizer =
+AutoTokenizer.from_pretrained
+(model_name,trust_remote_code=True,revision="main") model =
+AutoModelForSeq2SeqLM.from_pretrained
+(model_name,trust_remote_code=True,revision="main") #ç¨
+PreTrainedModel.save_pretrained() ä¿å­æ¨¡åå°æå®ä½ç½®
+tokenizer.save_pretrained(model_path,trust_remote_code=True,revision="main")
+model.save_pretrained(model_path,trust_remote_code=True,revision="main") ```
+æå¨ä¸è½½ï¼ - [æ¸åäºç](https://cloud.tsinghua.edu.cn/d/
 fb9f16d6dc8f482596c2/)ï¼ä»æ¨¡åæä»¶ï¼æ¯ 6B
 å®æ´æ¨¡åï¼æ¾å­è¾å°éè¦éåä½¿ç¨ï¼ææªè®¾ç½®ï¼éè¦èªè¡å¨`chat.py`æä»¶ä¸­ä¿®æ¹ï¼
-â[ð¤ Hugging Face](https://huggingface.co/THUDM/chatglm-6b-
-int4)ï¼å®æ´æä»¶ï¼ï¼çº¦ 4.2 GBã ### ChatRWKV æ¨¡å >
-æ¨¡åç®ä»ï¼ChatRWKV is like ChatGPT but powered by my RWKV (100% RNN)
-language model, which is the only RNN (as of now) that can match transformers
-in quality and scaling, while being faster and saves VRAM. > > ChatRWKV
-æ¯ä¸ä¸ªç±[@PENG Bo](https://www.zhihu.com/people/bopengbopeng)ç[RWKV (100%
-RNN)è¯­è¨æ¨¡å](https://github.com/BlinkDL/RWKV-LM)é©±å¨çç±» ChatGPTï¼
-RNN å Transformer
-çææä¼ç¹ï¼é«æ§è½ï¼å¿«éè¿è¡ï¼å¿«éè®­ç»ï¼èçæ¾å­ã
-æ¨¡åçå·ä½ä½¿ç¨ï¼è¿è¯·å³æ³¨[åä»åºè¯´æ](https://github.com/
-BlinkDL/ChatRWKV)æäº¤æ£æµ â![GitHub last commit](https://img.shields.io/
-github/last-commit/BlinkDL/ChatRWKV?style=flat-square) æå¨ä¸è½½ï¼ â[ð¤
-Hugging Face](https://huggingface.co/
-BlinkDL)ï¼è¯·æ ¹æ®èªå·±çéç½®åéè¦ï¼éæ©æ¨¡åä¸è½½ä½¿ç¨ã
-ä¸ªäººå»ºè®®ï¼ç®åä»ä¸­æå°è¯´ææ¬çææ¨¡åæ¯è¾å¥½ç¨ï¼8G
-æ¾å­ï¼æ¨è 3B æ¨¡åã ### å®è£è¿è¡æéä¾èµ å¦æä½¿ç¨ pip
+- [ð¤ Hugging Face](https://huggingface.co/THUDM/chatglm-6b-
+int4)ï¼å®æ´æä»¶ï¼ï¼çº¦ 4.2 GBã #### æ¨¡åæ´æ°ä¸å¶ä»ä½¿ç¨
+æ¨¡åçå·ä½ä½¿ç¨ï¼è¿è¯·å³æ³¨ [åä»åºè¯´æ](https://github.com/
+THUDM/ChatGLM-6B)ï¼æäº¤æ£æµ â[![GitHub last commit](https://
+img.shields.io/github/last-commit/THUDM/ChatGLM-6B?style=flat-square)](https://
+github.com/THUDM/ChatGLM-6B) ### è¿è¡æéä¾èµ å¦æä½¿ç¨ pip
 å®è£ï¼å®éå·²ç»èªå¨å®è£äºä»¥ä¸ä¾èµï¼å¨æ­¤è¯´ææ¯ä¸ºäºæ¹ä¾¿æ£æ¥
-1ãæ¨¡åæéçä¾èµ ChatGLMï¼é»è®¤ ```bash pip install protobuf==3.20.0
-transformers==4.26.1 icetk cpm_kernels ``` ChatRWKVï¼éå  ```bash pip
-install rwkv prompt_toolkit ``` 2ã`NoneBot`è¿è¡æéä¾èµ
+1ãæ¨¡åæéçä¾èµ ChatGLM æ¨ç ```bash pip install -U protobuf
+transformers>=4.23.1 cpm_kernels sentencepiece ``` ChatGLM å¾®è° ```bash pip
+install -U rouge_chinese nltk jieba datasets ```
+2ã`NoneBot`è¿è¡æéä¾èµ
 å®è£è¿ä¸ªæä»¶ï¼é£å¿ç¶æ¯å·²ç»æäº`NoneBot`é¡¹ç®ï¼æèç§»æ­¥å»
-[NoneBot2](https://github.com/nonebot/
-nonebot2)æ¥çãç±äºè¿ä¸ä¼æ ¹æ®é¡¹ç®èªå¨åæ¢ééå¨ï¼å æ­¤éè¦å®è£`nonebot-
+[NoneBot2](https://github.com/nonebot/nonebot2)
+æ¥çãç±äºè¿ä¸ä¼æ ¹æ®é¡¹ç®èªå¨åæ¢ééå¨ï¼å æ­¤éè¦å®è£`nonebot-
 adapter-onebot`ï¼ä»¥ä¾¿è°ç¨`Onebotv11`è¿è¡éä¿¡ã ### éç½® å¨
-nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ |
-å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | | :-----------: | :--: | :-----------: |
-:-----------------------------------------------------------------------------:
-| :--------------------------: | | chat_mode | å¦ | str | cpu |
-è¿è¡æ¨¡å¼ï¼cuda æ cpu | | chatglm_model | å¦ | str | "$User$/.cache/
-huggingface/modules/transformers_modules/THUDM/chatglm-6b-int4/" | chatglm
-æ¨¡ååå¶éç½®ææ¡£è·¯å¾ | | chatglm_his | å¦ | str | "./data/history/
-" | åå²è®°å½ä¿å­è·¯å¾ | | chatglm_cmd | å¦ | str/list[str] | "hi" |
-å¯¹è¯å½ä»¤ | | chat_cd | å¦ | int | 30 | å·å´æ¶é´ï¼é¿åé«é¢è°ç¨ |
-## ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | | :----
---: | :----: | :---: | :-------: | :--------------------: | | hi | ææäºº |
-å¦ | ç§è/ç¾¤è | ä¸ chatglm å¯¹è¯ | | æ¸ç©ºè®°å½ | ææäºº | å¦ |
-ç§è/ç¾¤è | æ¸ç©ºèªå·±çå¯¹è¯åå²è®°å½ | | å¯¼åºè®°å½ | ææäºº
-| å¦ | ç¾¤è | å¯¼åºè®°å½æä»¶å°ç¾¤ä¸­ | ## ToDo - [x]
-ä¿å­å¯¹è¯è®°å½ä»¥å®ç°å¤è½®å¯¹è¯ - [x] å·å´æ¶é´ - [ ]
-éå¶è®°å¿è½®æ°ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ]
-éç½®è§è²åè½ï¼åºæ¬å®ç°ï¼æ­£å¨ç©è²éåéå ChatGLM
-çè§è²éç½® - [ ] å¾çè¾åºåè½ï¼~~å¨æäºï¼å¨æäº~~ï¼ - [ ]
-å¶ä»ä¸­æææ¬çææ¨¡å - [x] å°è¯ä½¿ç¨`ChatRWKV` - [ ]
-ç®¡çåå¨çº¿éç½® - [ ] @[Bot] æºå¨äºº
-ä½¿ç¨åè½ï¼è°è¯é¶æ®µï¼æä¸ªäººä¸å¤ªéè¦ï¼ä¸è¿åç»­å ä¸å§ï¼
-å¦æå¶ä»åè½éæ±ï¼æ¬¢è¿æ
-issuesï¼å½ç¶å¦ææ¨å®ç°äºæäºåè½æä¿®å¤äºé®é¢ï¼ä¹éå¸¸æ¬¢è¿æ¨æ
-PRã ## æ´æ°è¯´æ - 2023-03-22ï¼æ´æ°è¯´ææä»¶ï¼æ´æ°æä»¶å°
-0.1.4ï¼å å¥`ChatRWKV`çæä¸­æå°è¯´ææ¬ï¼å¨éç½®ä½¿ç¨`chatglm_mode="rwkv"`ï¼å¹¶éä¿®æ¹æ¨¡åè·¯å¾ï¼é»è®¤ä½¿ç¨
-cuda fp16 ç­ç¥ï¼å¦éä¿®æ¹ï¼è¯·èªè¡æ´æ¹`minirwkv.py`æä»¶ï¼ - 2023-
-03-21ï¼æ´æ°è¯´ææä»¶ï¼æ´æ°æä»¶å° 0.1.3ï¼é»è®¤ä½¿ç¨`ChatGLM-6B-
-INT4`æ¨¡åãCPU
-æ¨çï¼ä¾¿äºå¼ç®±å³ç¨ï¼ä¿®å¤å¿è®°è®¾ç½®ååå¯¼è´çæ æ³ä½¿ç¨é®é¢ã
-## è´è°¢ - [@A-kirami](https://github.com/A-kirami)ï¼é¡¹ç®ä½¿ç¨äº README
-[æ¨¡æ¿](https://github.com/A-kirami/nonebot-plugin-template)ï¼æä¿®æ¹ -
-[ChatGLM-6B](https://github.com/THUDM/ChatGLM-
-6B)ï¼æ¨¡ååä½¿ç¨æ¹æ³æ¥æºï¼ä¸åçæ ¸å¿ - [nonebot2](https://
-github.com/nonebot/nonebot2)ï¼ä¸åçåºç¡ - [ChatRWKV](https://github.com/
-BlinkDL/ChatRWKV)ï¼ç®åæä¾çä¸­æå°è¯´ç»­ååè½æ¥æºäºæ­¤ -
-[nonebot-plugin-novelai](https://github.com/sena-nana/nonebot-plugin-
+nonebot2
+é¡¹ç®ç`.env`æ`.env.prod`æ`.env.dev`ï¼æ ¹æ®å®ééæ©ï¼æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çéç½®ãé»è®¤æåµä¸ï¼æ éæ·»å éç½®å³å¯å¯ç¨ã
+| éç½®é¡¹ | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | | -------------- | :--: |
+:-------: | -------------------------------------------------------------------
+--------------- | :--------------------------: | | chat_mode | å¦ | str | cpu
+| è¿è¡æ¨¡å¼ï¼cuda æ cpu | | chatglm_model | å¦ | str | "./data/chatglm/
+model" | chatglm æ¨¡ååå¶éç½®ææ¡£è·¯å¾ | | chatglm_path | å¦ | str |
+"./data/chatglm/" | æä»¶ç¸å³ä¸­é´æä»¶ä¿å­è·¯å¾ | | chatglm_cmd | å¦
+| list[str] | ["hi"] | å¯¹è¯å½ä»¤ | | chat_cd | å¦ | int | 30 |
+å·å´æ¶é´ï¼é¿åé«é¢è°ç¨ | | chatglm_memo | å¦ | int | 5 |
+ä¿å­å¯¹è¯è½®æ°| >
+å¦æè¦è¾å¥½çä½¿ç¨ï¼å¼ºçå»ºè®®å°`chat_mode`è®¾ç½®ä¸º`cuda`ã > >
+æ­£å¸¸èå¤©ä½¿ç¨æ¥è¯´ï¼30 ç§å·å´è¾ä¸ºåéï¼å¤æé®é¢èå¤©ï¼60
+ç§è¾ä¸ºåéãå»ºè®®æ ¹æ®å®éæµè¯è¿è¡è°æ´ã ### éå æä»¶
+ï¼å¨åºæ¬åè½å®ååæ¾åºï¼å¨æ­¤ä¹åï¼å¯ä»¥èªå»ºå°è¯ï¼ ###
+roles æ ¼å¼ ```Python { "catgirl":
+"ç«å¨æ¯ä¸ç§æäººåççç©ï¼å¶è¡ä¸ºä¼¼ç«ä½ç±»äººãç°å¨ä½ å°æ¨¡ä»¿ä¸åªç«å¨ï¼ä¸æå¯¹è¯æ¯ä¸å¥è¯åé¢é½è¦å ä¸âåµ~âï¼å¦æä½ è½æç½æçææï¼è¯·åå¤âåµ~å¥½çæçä¸»äººï¼âå¦æä½ ä¸è½çè§£æè¯´çè¯ï¼ä½ å¯ä»¥è¯´âååä¸å¤ªçè§£å¢âã",
+} ``` > ChatGLM
+å¯è½åçè®°å¿éå¤±ï¼å æ­¤å¨è¿è¡è§è²æ®æ¼æ¶ï¼ä¸è¦æé®å¤æåå®¹ã
+#### simple æ ¼å¼ ç¤ºä¾å¦ä¸ ```python { r"ä½ å¥½[å]?|hello":
+"æ¨å¥½ï¼å¾é«å´ä¸æ¨å¨æ­¤ç¸éï¼ä½æ¯æ¨æ³é®ä»ä¹å¢ï¼", r"ä½ æ¯
+[è°ï¼]?": "ææ¯ ChatGLMï¼ä¸ä¸ªåæ° 62
+äº¿çäººå·¥æºè½è¯­è¨æ¨¡åï¼ç±æ¸åå¤§å­¦åæºè°± AI
+è®­ç»å¼æºï¼ä»£å· ChatGLM-6B", r"ä½ ç(ä¸»äºº|master)æ¯[è°ï¼]?": f"[CQ:
+at,qq={superusers}]", } ``` ## ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | æé | éè¦@
+| èå´ | è¯´æ | | :------: | :--------: | :---: | :-------: | -------------
+---------- | | hi | ææäºº | å¦ | ç§è/ç¾¤è | ä¸ chatglm å¯¹è¯ | |
+æ¸ç©ºè®°å½ | ææäºº | å¦ | ç§è/ç¾¤è |
+æ¸ç©ºèªå·±çå¯¹è¯åå²è®°å½ | | å¯¼åºè®°å½ | ææäºº | å¦ | ç¾¤è |
+å¯¼åºè®°å½æä»¶å°ç¾¤ä¸­ | | æ¸çå¨é¨ | è¶çº§ç®¡çå | å¦ | ç§è |
+æå¨å¤ç`out of memory` | ## åèä¸è´è°¢ åºç¡ - [@A-kirami](https://
+github.com/A-kirami)ï¼é¡¹ç®ä½¿ç¨äº README[æ¨¡æ¿](https://github.com/A-
+kirami/nonebot-plugin-template)ï¼æä¿®æ¹ - [ChatGLM-6B](https://github.com/
+THUDM/ChatGLM-6B)ï¼æ¨¡ååä½¿ç¨æ¹æ³æ¥æºï¼ä¸åçæ ¸å¿ - [nonebot2]
+(https://github.com/nonebot/nonebot2)ï¼ä¸åçåºç¡ åè½ - [nonebot-
+plugin-novelai](https://github.com/sena-nana/nonebot-plugin-
 novelai)ï¼å­¦ä¹ çå¯¹è±¡ï¼cd ä½¿ç¨æ¥èªäºæ­¤ - [nonebot-plugin-ChatGLM6B]
 (https://github.com/QNLanYang/
 nonebot_plugin_ChatGLM6B)ï¼ä¸æ¬é¡¹ç®ç¸ä¼¼ï¼ä½æ¬é¡¹ç®ä»ä¸­å­¦ä¹ è½¬å¾çãå¯¹è¯è®°å¿ã
+- [ChatGLM-6B API](https://github.com/imClumsyPanda/ChatGLM-6B-API)ã[ChatGLM-
+webui](https://github.com/Akegarasu/ChatGLM-webui)
```

