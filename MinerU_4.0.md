# MinerU 4.0

MinerU 4.0 brings document parsing, a local document library, and service tools into one workflow for document conversion, application integration, and agent reading.

## Four Parsing Tiers

- **Flash** — for fast previews and indexing
- **Basic** — for OCR and model-based parsing
- **Standard / Advanced** — for more demanding layouts and quality requirements

## Multiple Input Formats

PDF, images, DOC/DOCX, PPT/PPTX, XLS/XLSX, RTF, ODT/ODS/ODP, EPUB, OFD, HTML/MHTML, and CSV/TSV. DocVortex provides native document parsing.

## Document Library and Agent Reading

- Discover files
- Cache results
- Search content
- Continue by page or block
- Preserve stable citation locators

## Independent Model Configuration

- **Small models:** ONNX or Torch
- **VLM:** llama.cpp, vLLM, or LMDeploy

## Unified Tools

- Python SDK
- V1 API
- Stateless batch conversion
- Multi-service Router
- Gradio-based WebUI

## Structured Results and Rendering

One document model supports **nine rendering targets**:

1. Markdown
2. HTML
3. LaTeX
4. DOCX
5. EPUB
6. PDF
7. Structured Content
8. Content List V1
9. Content List V2

Each CLI/API exposes its own subset of exports; see Output Formats and Result Contract.

## Format Support and Parsing Notes

| Format | Parsing Tier / Method |
| --- | --- |
| PDF and images | All four tiers (Flash / Basic / Standard / Advanced) |
| Office (DOC/DOCX, PPT/PPTX, XLS/XLSX), RTF, ODT/ODS/ODP | Local Flash native parsing |
| EPUB, OFD | Local Flash native parsing |
| HTML/MHTML | Local Flash native parsing |
| CSV/TSV | Local Flash native parsing |
| Plain text | Read directly (not parsed) |

> Documents are not automatically uploaded to the official service; remote parsing requires explicit configuration.