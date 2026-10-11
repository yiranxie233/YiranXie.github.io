---
permalink: /
title: "解一然｜大模型应用与智能体开发"
excerpt: "聚焦 RAG 知识库、LangGraph 多智能体系统与可信大模型应用落地。"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<div class="profile-lead" markdown="1">

我是一名面向实际业务问题的大模型应用开发者，关注 **RAG 知识库、LangGraph 多智能体编排、模型服务工程化与可信内容生成**。我习惯把一个想法推进为可以验证的完整闭环：从数据解析与检索评测，到后端接口、状态管理和前端交互。

硕士毕业于上海电力大学电子信息（新一代电子信息技术）专业，GPA 4.21/5、专业排名前 5%。除智能体应用外，我也有 PyTorch、CLIP 多模态深度学习研究经历。

</div>

[查看项目经历]({{ '/teaching/' | relative_url }}){: .btn .btn--primary }
[了解个人背景]({{ '/cv/' | relative_url }}){: .btn }
[浏览论文成果]({{ '/publications/' | relative_url }}){: .btn }

## 项目成果概览

<div class="impact-grid">
  <div class="impact-card">
    <strong>94.02%</strong>
    <span>RAG 检索 MRR@5</span>
    <small>50+ 并发会话，P99 延迟 1.2s</small>
  </div>
  <div class="impact-card">
    <strong>99.8%</strong>
    <span>旅行规划端到端有效成功率</span>
    <small>景点事实与有效坐标率均为 100%</small>
  </div>
  <div class="impact-card">
    <strong>87%</strong>
    <span>岗位 HR 信息解析准确率</span>
    <small>覆盖采集、解析、生成与导出闭环</small>
  </div>
</div>

## 精选项目

### [智能简历项目制作助手]({{ '/teaching/resume-project-agent/' | relative_url }})

使用 LangGraph、FastMCP 与 PostgreSQL 构建本地优先的简历智能体，串联岗位采集、JD 拆解、简历解析、多维匹配、人工确认和多格式导出，并对模型推导内容提供“待核实”标记与逐字段确认。

### [智能旅行规划助手]({{ '/teaching/ai-travel-planner/' | relative_url }})

将景点、天气、酒店和行程规划拆分为协作 Agent，通过高德 MCP 获取真实外部数据，以 Pydantic 约束结构化输出，并用 FastAPI SSE 与 Vue 3 完成地图展示闭环。

### [智能 RAG 知识库问答助手]({{ '/teaching/rag-knowledge-base/' | relative_url }})

围绕 PDF 版面解析、FAISS + BM25 混合召回、Qwen3-Reranker 重排、答案溯源和多用户数据隔离优化知识库问答链路，检索答案均可追溯至源文档。

[查看全部 5 个项目 →]({{ '/teaching/' | relative_url }}){: .btn .btn--primary }

## 核心技术栈

<div class="tech-cloud">
  <span class="tech-chip">Python</span>
  <span class="tech-chip">LangChain</span>
  <span class="tech-chip">LangGraph</span>
  <span class="tech-chip">FastAPI</span>
  <span class="tech-chip">RAG</span>
  <span class="tech-chip">FAISS</span>
  <span class="tech-chip">BM25</span>
  <span class="tech-chip">FastMCP / MCP</span>
  <span class="tech-chip">PostgreSQL</span>
  <span class="tech-chip">PyTorch</span>
  <span class="tech-chip">Docker</span>
</div>

## 当前关注

- 让智能体工作流具备可恢复状态、人工确认节点和可追踪的事实边界。
- 用混合检索、重排与检索评测提升中文 RAG 的召回质量和回答可信度。
- 将模型能力封装为稳定、可观察、可接入前端业务的工程服务。
