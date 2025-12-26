# AIOT_HW5

## 🎬 n8n 自動化短影音生成器 (Automated Short Video Generator)

[![Demo Video]([https://img.shields.io/badge/Demo-Watch%20Video-red](https://github.com/user-attachments/assets/1c5a2f35-472d-4dda-851d-bee0d69bda09))]


https://github.com/user-attachments/assets/67076fc4-7ee8-46d2-a14a-a7302bdc979c



## 📖 專案簡介 (Introduction)

本專案旨在展示如何透過 **n8n** 自動化工作流程，將一個簡單的主題概念轉化為引人入勝的短影音。利用生成式 AI 的強大功能，從腳本撰寫、素材生成到最終的影片剪輯，實現完全自動化的內容創作流程。

## ⚙️ 運作流程 (Workflow)

整個自動化流程分為三個主要階段：

### 1. 📝 AI 腳本與視覺描述生成 (Script & Prompt Generation)
在此階段，我們使用大型語言模型 (LLM) 來構思內容：
- **產生腳本**：根據輸入的主題，生成分鏡腳本與旁白內容。
- **產生提示詞**：為每一個分鏡場景生成精確的圖像生成提示詞 (Image Prompts)。

### 2. 🎨 素材生成 (Asset Generation)
利用第三方 API 將文字轉化為視聽素材：
- **圖像生成**：呼叫繪圖模型 (如 DALL-E 3, Midjourney API, Stable Diffusion) 產生場景圖。
- **影片生成**：將圖像轉為動態影片 (Image-to-Video)。
- **語音生成**：透過 TTS (Text-to-Speech) 服務 (如 OpenAI, ElevenLabs) 將旁白轉為語音檔案。

### 3. 🎬 影片合成 (Video Assembly)
將上述生成的所有片段組合在一起：
- **整合**：將對應的影片片段與音檔進行對齊。
- **輸出**：透過影片處理工具 (如 FFmpeg) 合成為一段完整的短影音 (MP4)。


