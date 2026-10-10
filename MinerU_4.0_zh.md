# MinerU 4.0

MinerU 4.0 将文档解析、本地文档库和服务工具整合到同一工作流中，可用于文档转换、应用集成以及智能体（Agent）阅读。

## 四级解析

- **Flash（极速）** — 适用于快速预览和索引
- **Basic（基础）** — 适用于 OCR 和基于模型的解析
- **Standard / Advanced（标准 / 高级）** — 适用于更复杂的版面和更高的质量要求

## 多种输入格式

PDF、图片、DOC/DOCX、PPT/PPTX、XLS/XLSX、RTF、ODT/ODS/ODP、EPUB、OFD、HTML/MHTML 以及 CSV/TSV。DocVortex 提供原生文档解析。

## 文档库与智能体阅读

- 发现文件
- 缓存结果
- 搜索内容
- 按页或按块继续阅读
- 保留稳定的引用定位符

## 独立的模型配置

- **小模型：** ONNX 或 Torch
- **VLM（视觉语言模型）：** llama.cpp、vLLM 或 LMDeploy

## 统一的工具

- Python SDK
- V1 API
- 无状态批量转换
- 多服务路由器（Router）
- 基于 Gradio 的 WebUI

## 结构化结果与渲染

单一文档模型支持**九种渲染目标**：

1. Markdown
2. HTML
3. LaTeX
4. DOCX
5. EPUB
6. PDF
7. 结构化内容（Structured Content）
8. 内容列表 V1（Content List V1）
9. 内容列表 V2（Content List V2）

每个 CLI/API 均提供各自支持的部分导出格式；详见"输出格式"与"结果契约"。

## 格式支持与解析说明

| 格式 | 解析级别 / 方式 |
| --- | --- |
| PDF 和图片 | 全部四级（Flash / Basic / Standard / Advanced） |
| Office 文档（DOC/DOCX、PPT/PPTX、XLS/XLSX）、RTF、ODT/ODS/ODP | 本地 Flash 原生解析 |
| EPUB、OFD | 本地 Flash 原生解析 |
| HTML/MHTML | 本地 Flash 原生解析 |
| CSV/TSV | 本地 Flash 原生解析 |
| 纯文本 | 直接读取（不做解析） |

> 文档不会自动上传至官方服务；远程解析需要显式配置。
