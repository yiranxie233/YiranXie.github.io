---
title: "本地化智能问答系统"
collection: teaching
type: "RAG"
permalink: /teaching/2014-spring-teaching-1
venue: "Langchain, Gradio, BM25, Reranker"
date: 2025-07-15
location: "广东-深圳"
---
- 负责搭建文档知识库处理流程，支持 PDF、Word、Excel、PPT、TXT、Markdown 等多格式文件解析、文本切分、向量化及索引构建。
- 采用 FAISS 语义检索与 BM25 关键词检索相结合的混合召回策略，并结合 Cross-Encoder 重排序，提高复杂问题下的检索相关性。
- 设计递归检索与查询改写机制，根据初始检索结果动态生成后续查询，增强多跳问题和信息不足场景下的回答能力。
- 集成本地 Ollama 及 SiliconFlow、Magick、DMX 等云端大模型，统一封装调用接口，并实现模型自动检测与故障回退。
- 开发 Gradio 交互式问答界面和 FastAPI 服务接口，支持联网搜索、来源标注、多来源矛盾检测及用户知识库隔离。
