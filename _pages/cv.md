---
layout: archive
title: "个人简介"
permalink: /cv/
excerpt: "解一然的教育背景、技术能力、项目方向与学术成果。"
author_profile: true
redirect_from:
  - /resume
---
{% include base_path %}

## 个人定位

大模型应用与智能体开发方向，熟练使用 Python、LangChain、LangGraph 构建 RAG 知识库和多 Agent 系统，具备从文档解析、混合检索、重排优化到后端接口与前端展示的完整项目实践。

## 教育背景

### 上海电力大学 · 电子信息（新一代电子信息技术）硕士

2023.09–2026.06 · GPA 4.21/5，专业排名前 5%

主修课程：机器学习、矩阵论、现代数字信号处理技术、传感器技术。

### 太原工业学院 · 电子信息工程学士

2019.09–2023.07 · GPA 3.88/5，专业排名前 5%

主修课程：信号与系统、线性代数、数字电路、数字信号处理、单片机。

## 技术能力

- **熟练掌握：** Python、LangChain、LangGraph、PyTorch
- **熟悉使用：** Linux、SQL、FastAPI、爬虫
- **项目实践：** FAISS、BM25、SQLite、PostgreSQL、FastMCP / MCP、Streamlit、Playwright、PaddleOCR、Ollama、Docker、Vue 3

## 代表项目

- [智能简历项目制作助手]({{ '/teaching/resume-project-agent/' | relative_url }})：围绕“一岗一简历”构建岗位采集、JD 拆解、简历结构化、匹配评分、候选生成、人工确认与文件导出的端到端 MVP。
- [智能旅行规划助手]({{ '/teaching/ai-travel-planner/' | relative_url }})：基于 LangGraph 与 MCP 的多 Agent 旅行规划系统，结构化输出成功率 99.2%，端到端有效成功率 99.8%。
- [智能 RAG 知识库问答助手]({{ '/teaching/rag-knowledge-base/' | relative_url }})：优化 PDF 解析、混合检索、重排、答案溯源与多用户隔离，支持 50+ 并发会话。
- [环境光自适应河道垃圾检测系统]({{ '/teaching/river-waste-detection/' | relative_url }})：获第十九届中国研究生电子设计大赛三等奖。

[查看完整项目经历]({{ '/teaching/' | relative_url }}){: .btn .btn--primary }

## 奖励与成果

- 校长奖学金，2026.04
- 学业成果一等奖学金，2026.04
- 研究生阶段课程一等奖学金，2024.12
- 第十九届中国研究生电子设计大赛三等奖，2024.07
- 研究生入学成绩一等奖学金，2023.10
- 第十四届全国大学生数学竞赛（非数学类）二等奖，2023.01

## 论文成果

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>
