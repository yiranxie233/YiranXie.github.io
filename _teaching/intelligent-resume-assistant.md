---
title: "智能简历项目制作助手"
collection: teaching
type: "Agent / 简历工具"
permalink: /teaching/resume-project-agent/
date: 2026-08-01
period: "2026.08-2026.10"
role: "项目构建：端到端智能体工作流与产品实现"
stack:
  - Python
  - FastAPI
  - Streamlit
  - LangChain
  - LangGraph
  - FastMCP
  - PostgreSQL
  - Playwright
  - PaddleOCR
  - Ollama
venue: "本地优先简历智能体"
link: "https://github.com/yiranxie233/resume-agent"
excerpt: "面向“一岗一简历”场景，覆盖岗位采集、JD 拆解、简历解析、匹配评分、候选生成、人工核实与多格式导出。"
---

## 项目背景

面向“一岗一简历”求职场景搭建本地优先的简历智能体，解决岗位 JD 与简历项目匹配不足、定制修改耗时、生成内容缺少事实校验以及修改时容易破坏排版等问题。

## 核心工作 / 方案

- 基于 LangGraph 将环境配置、JD 解析、简历结构化、岗位多维匹配、候选生成、人工确认和文件导出拆分为状态节点，通过 `thread_id` 与 PostgreSQL checkpoint 保存任务上下文。
- 以 FastMCP 的 stdio 模式封装 BOSS 岗位采集工具，使用独立 Edge Profile 复用登录态，实现岗位卡片增量加载、HR 姓名与活跃时间提取及后台详情解析。
- 接入 PaddleOCRv6，支持岗位截图粘贴或上传、文字校正及大模型进一步解析。
- 分离云端、本地大模型和 Embedding 模型配置，兼容 OpenAI 格式接口与 Ollama 动态模型发现；使用 Pydantic 约束 JD、简历和候选项目的结构化输出。
- 围绕技能、职责、项目和关键词进行匹配，默认生成 3 个可编辑候选项目，并为模型推导内容增加“待核实”标记和逐字段确认。
- 支持 Word、Markdown、PDF 的解析、预览和结构校正，并通过 Gitee FastMCP 搜索 Word 模板供用户预览和选择。

## 量化成果

- 完成岗位采集、JD 拆解、项目生成、简历修改和文件导出的端到端 MVP。
- HR 名称和活跃时间解析准确率达到 87%。
- 支持候选不足时保留已有结果并自动补齐，以及对生成内容进行反馈、编辑、核实和版本追踪。

## 技术栈

Python、FastAPI、Streamlit、LangChain、LangGraph、FastMCP、PostgreSQL、Playwright、PaddleOCR、Ollama。
