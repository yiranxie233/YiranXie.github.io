---
title: "智能旅行规划助手"
collection: teaching
type: "Multi-Agent / 旅行规划"
permalink: /teaching/ai-travel-planner/
date: 2026-06-01
period: "2026.06-2026.08"
role: "项目参与：多 Agent 工作流与前后端闭环"
stack:
  - Python
  - FastAPI
  - LangChain
  - LangGraph
  - MCP
  - Vue 3
  - Pydantic
  - Docker
venue: "多 Agent 智能行程规划系统"
excerpt: "由景点、天气、酒店和规划 Agent 协作，完成多源信息检索、结构化行程生成、地图展示与导出闭环。"
redirect_from:
  - /teaching/2015-spring-teaching-1
---

## 项目背景

参与面向自由行用户的多 Agent 智能行程规划系统建设，解决旅行信息碎片化、生成行程缺少真实外部数据支撑、输出格式不稳定及难以对接前端地图组件等问题。

## 核心工作 / 方案

- 将系统拆分为景点搜索、天气查询、酒店推荐和行程规划 4 个角色；3 个资料 Agent 通过高德 MCP 工具检索，规划 Agent 统一整合结果。
- 使用 Pydantic 定义业务领域模型并执行运行时校验，约束行程时间区间、归一化温度单位并过滤越界经纬度。
- 前端完成目的地、时间、偏好标签等 6 项信息采集，展示行程、住宿、预算和地图等内容，并支持景点调整及图片、PDF 导出。
- 使用 FastAPI 实现 SSE 流式返回并以 Docker 容器化部署；通过模型懒加载和本地缓存优化响应速度与 Token 开销。

## 量化成果

- 结构化输出成功率达到 99.2%，端到端有效成功率达到 99.8%。
- 行程景点信息、坐标与高德检索数据的事实一致率以及有效坐标率均达到 100%。
- P99 延迟优化至 1.7s，单次请求 Token 成本下降 30%。

## 技术栈

Python、FastAPI、LangChain、LangGraph、MCP、Vue 3、Pydantic、Docker。
