# 🚀 Modular RAG Framework (LangGraph + Chroma + Pluggable LLM)
一个可插拔 LLM 的 RAG 框架模板
支持多模型切换、持久化向量库、可扩展插件层
可用于教学、实验对比或生产级扩展

📌 项目简介

本项目实现了一个模块化 RAG（Retrieval-Augmented Generation）系统，具有以下特点：

✅ 基于 LangGraph 的流程编排

✅ 使用 Chroma 持久化向量数据库

✅ 支持 可插拔 LLM 架构

✅ 支持离线运行（FakeLLM / SimpleEmbedding）

✅ 支持 OpenAI-compatible API（AIHubMix / OpenRouter 等）

✅ 支持本地模型（Ollama）

本项目旨在：

提供一个结构清晰、可扩展、可对比不同 LLM 效果的 RAG 框架模板。

🧱 技术栈（Tech Stack）

🔹 框架层

LangChain	LLM 抽象接口 & Prompt 管理

LangGraph	有状态流程编排（Stateful Workflow）

Python 3.12	运行环境

🔹 检索层（Retrieval Layer）

Chroma，本地持久化向量数据库

RecursiveCharacterTextSplitter，文档分块

Embeddings (可插拔)，	支持 SimpleEmbedding / 真实Embedding

🔹 生成层（Generation Layer）

支持多种 LLM：

FakeLLM（离线测试）

Ollama（本地模型）

OpenAI-compatible（AIHubMix / OpenRouter）

其他 API

🔹 可扩展插件层

可扩展模块包括：

Rerank 插件层

Embedding 插件层

Evaluation 节点

多轮 Query Rewrite

Fallback 节点

Agent Tool 插件层

📁 项目结构


