# MinerU 4.0

MinerU 4.0 将文档解析、本地文档库和服务工具整合到统一工作流中，用于文档转换、应用集成和智能体（Agent）阅读。

## 四个解析级别

- **Flash（极速）** —— 用于快速预览和索引
- **Basic（基础）** —— 用于 OCR 和基于模型的解析
- **Standard / Advanced（标准/高级）** —— 用于更复杂的版面布局和更高的质量要求

## 多种输入格式

支持 PDF、图片、DOC/DOCX、PPT/PPTX、XLS/XLSX、RTF、ODT/ODS/ODP、EPUB、OFD、HTML/MHTML 以及 CSV/TSV。DocVortex 提供原生文档解析。

## 文档库与智能体阅读

- 发现文件
- 缓存解析结果
- 搜索内容
- 按页或按区块继续读取
- 保留稳定的引用定位符

## 独立的模型配置

- **小型模型：** ONNX 或 Torch
- **VLM（视觉语言模型）：** llama.cpp、vLLM 或 LMDeploy

## 统一的工具

- Python SDK
- V1 API
- 无状态批量转换
- 多服务路由器（Multi-service Router）
- 基于 Gradio 的 WebUI

## 结构化结果与渲染

单一文档模型支持 **九种渲染目标**：

1. Markdown
2. HTML
3. LaTeX
4. DOCX
5. EPUB
6. PDF
7. Structured Content（结构化内容）
8. Content List V1（内容列表 V1）
9. Content List V2（内容列表 V2）

每个 CLI/API 仅暴露各自的导出子集；详见“输出格式”与“结果契约”。

## 格式支持与解析说明

| 格式 | 解析级别 / 方法 |
| --- | --- |
| PDF 和图片 | 全部四个级别（Flash / Basic / Standard / Advanced） |
| Office（DOC/DOCX、PPT/PPTX、XLS/XLSX）、RTF、ODT/ODS/ODP | 本地 Flash 原生解析 |
| EPUB、OFD | 本地 Flash 原生解析 |
| HTML/MHTML | 本地 Flash 原生解析 |
| CSV/TSV | 本地 Flash 原生解析 |
| 纯文本 | 直接读取（不经过解析） |

> 文档不会自动上传至官方服务；远程解析需要进行显式配置。
