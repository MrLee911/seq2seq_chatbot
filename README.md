# 🤖 Seq2Seq Chatbot with PyTorch

本项目是一个使用 PyTorch 实现的中文对话机器人，基于经典的 Seq2Seq 编码器-解码器结构（LSTM），支持命令行交互与 Web 聊天界面。

## 📦 项目结构

```
seq2seq_chatbot/
├── vocab.py              # 词表类
├── dataset.py            # 数据加载
├── model.py              # 编码器-解码器模型
├── train.py              # 模型训练
├── evaluate.py           # BLEU评估 + 推理
├── utils.py              # 模型保存、加载、时间打印等
├── chat.py               # 命令行聊天界面
├── chat_gradio.py        # Web聊天界面（Gradio）
├── data/                 # 存放处理后的训练数据（已忽略）
├── DoubanConversationCorpus/ # 原始语料（已忽略）
```

## 🚀 使用步骤

### 1. 安装依赖

```bash
pip install -r requirements.txt
```

### 2. 数据预处理

```bash
python preprocess.py
```

### 3. 训练模型

```bash
python train.py
```

### 4. 聊天体验

```bash
# 命令行
python chat.py

# 或使用 Web 界面（推荐）
python chat_gradio.py
```

## 📊 模型与评估

- 编码器-解码器结构：LSTM
- 训练数据：豆瓣对话语料（建议自备）
- 评估指标：BLEU

## 📎 项目特点

- ✅ 支持 GPU 训练
- ✅ 结构简洁易懂，适合教学
- ✅ 支持命令行 + Web 聊天界面
- ✅ 词表支持自定义特殊符号（<sos>, <eos>, <unk>, <pad>）

---

本项目仅用于学习和教学用途，欢迎 star & fork 🌟
