# ai-qa-demo
“本地知识库问答机器人”
# 本地知识库问答机器人

[![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.95.0-green)](https://fastapi.tiangolo.com/)
[![LangChain](https://img.shields.io/badge/LangChain-0.1.0-orange)](https://www.langchain.com/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28.0-red)](https://streamlit.io/)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

> 基于 RAG（检索增强生成）的智能问答系统，支持上传本地文档，通过向量检索与大模型结合，实现精准、快速的上下文问答。

## ✨ 功能特点

- 📄 **多格式文档支持**：支持上传 TXT、PDF、Markdown 等格式文件，自动解析并建立索引。
- 🔍 **精准检索**：基于向量数据库（Chroma）实现语义搜索，快速定位相关内容。
- 🤖 **智能生成**：调用大语言模型 API，结合检索结果生成高质量答案。
- 🌐 **Web 交互界面**：使用 Streamlit 构建简洁易用的前端，支持文档上传、实时问答。
- ⚡ **快速响应**：平均响应时间 < 3 秒，提供流式输出体验。

## 🛠️ 技术栈

| 模块       | 技术选型                          |
|------------|-----------------------------------|
| 后端框架   | FastAPI                           |
| 前端界面   | Streamlit                         |
| 检索框架   | LangChain                         |
| 向量数据库 | Chroma（本地持久化）              |
| 嵌入模型   | text-embedding-ada-002（OpenAI）  |
| 大语言模型 | OpenAI GPT / 国内兼容 API         |
| 部署       | 阿里云 ECS（示例）                |

## 🚀 在线演示

> 如果已部署，可点击体验：[http://your-server-ip:8501](http://your-server-ip:8501)  
> 未部署时可忽略此项，直接本地运行。

## 📸 效果截图

### 文档上传界面
![文档上传](images/upload.png)

### 问答示例
![问答示例](images/qa.png)

## 📦 快速开始（本地运行）

### 1. 克隆项目
```bash
git clone https://github.com/your-username/local-rag-chatbot.git
cd local-rag-chatbot
