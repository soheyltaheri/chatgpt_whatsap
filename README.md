# WhatsApp ChatGPT AI Assistant

<p align="center">
  <strong>Automated WhatsApp AI Agent with Ambient Context & Real-Time OpenAI Integration</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10%2B-3776AB.svg?logo=python&logoColor=white" alt="Python Version" />
  <img src="https://img.shields.io/badge/OpenAI-GPT--4o--mini-412991.svg?logo=openai&logoColor=white" alt="OpenAI" />
  <img src="https://img.shields.io/badge/WhatsApp-Gateway%20API-25D366.svg?logo=whatsapp&logoColor=white" alt="WhatsApp" />
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License" />
</p>

---

## 📌 Overview

**WhatsApp ChatGPT AI Assistant** is a lightweight Python service that bridges WhatsApp messaging gateways with OpenAI language models. It provides real-time intelligent auto-responses, context-aware conversational flows, and dynamic telemetry ingestion (CPU, memory, system uptime, and ambient environment metrics).

---

## 🌟 Features

- 💬 **Intelligent Auto-Replies:** Bi-directional bridge between incoming WhatsApp messages and OpenAI chat completions.
- 🌍 **Bilingual Support:** Automatically responds in Persian or English matching the user's input language.
- 📊 **Ambient Data Telemetry:** Seamlessly queries host system metrics (CPU load, RAM consumption, OS runtime) and injects them into LLM context when prompted.
- 🛡️ **Defensive Error Handling:** Automatic reconnection, exponential backoff polling, and structured JSON parsing.

---

## 🚀 Quickstart & Setup

### 1. Installation
```bash
git clone https://github.com/soheyltaheri/chatgpt_whatsap.git
cd chatgpt_whatsap
pip install -r requirements.txt
```

### 2. Environment Configuration
Copy `.env.example` to `.env`:
```bash
cp .env.example .env
```

Set your API credentials:
```env
OPENAI_API_KEY=your_openai_api_key_here
OPENAI_MODEL=gpt-4o-mini
MESSAGE_WALL_API=your_gateway_api_key_here
MESSAGE_WALL_BASE_URL=https://api.chat-api.com
INSTANCE_ID=your_instance_id
POLL_INTERVAL_SECONDS=3
```

### 3. Execution
```bash
python auto_whatsap.py
```

---

## 📄 License
This repository is open-source and available under the [MIT License](LICENSE).
