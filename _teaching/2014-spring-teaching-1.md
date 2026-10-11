---
title: "智能 RAG 知识库问答助手"
collection: teaching
type: "RAG / 知识库问答"
permalink: /teaching/rag-knowledge-base/
date: 2025-07-01
period: "2025.07-2026.05"
role: "项目参与：RAG 全链路优化"
stack:
  - Python
  - LangChain
  - Qwen3
  - FAISS
  - BM25
  - SQLite
  - pdfminer
  - pdfplumber
  - Reranker
venue: "青岛博慧达电子科技有限公司"
excerpt: "面向中文 PDF 知识库问答，优化文档解析、混合检索、重排、答案溯源与多用户数据隔离的完整链路。"
redirect_from:
  - /teaching/2014-spring-teaching-1
---

## 项目背景

参与知识库问答 RAG 系统建设，针对传统 RAG 中 PDF 解析顺序错乱、表格结构丢失、检索精度不足、多用户数据未隔离以及回答无法溯源等问题，优化文档处理、检索召回、权限与来源标注链路。

## 核心工作 / 方案

- 重构 PDF 解析链路：融合 pdfminer 与 pdfplumber，分离提取正文和表格；通过坐标去重、阈值过滤页眉页脚及双栏布局自适应识别，改善文档顺序和表格结构问题。
- 完善中文检索链路：基于 Qwen3 系列中文模型，以 FAISS 语义检索和 BM25 关键词检索构建混合召回，并加入 Reranker、模型懒加载、本地缓存、多轮查询改写与校验。
- 加强答案溯源：将来源文件、页码和切片索引写入生成上下文，通过 Prompt 约束模型基于证据回答并标注来源。
- 实现多账户隔离：基于 SQLite 搭建用户体系，按用户独立存储知识库数据，并通过线程锁规避串库风险。

## 量化成果

- 中文文档语义割裂率下降约 60%，检索答案 100% 可追溯至源文档。
- Qwen3-Reranker 的 Page Hit@1 为 90.21%，Page Hit@5 为 93.64%，MRR@5 为 94.02%。
- 支持 50+ 并发会话，P99 延迟优化至 1.2s，单次查询 Token 成本降低 25%。

## 技术栈

Python、LangChain、Qwen3、FAISS、BM25、SQLite、pdfminer、pdfplumber、Reranker。
