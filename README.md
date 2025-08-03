# 🧠 AI-Powered Chat Summarizer Bot (n8n Workflow)

This repository contains an **n8n automation workflow** that receives chat messages, processes them using **OpenAI GPT-4.1-mini**, enriches context with **memory and SERP search**, summarizes the result, and sends a response to **Discord** via webhook.

---

## 📌 Features

- 🤖 Responds to incoming chat messages using an **AI Agent**
- 🧠 Maintains context using a **Memory Buffer**
- 🔎 Uses **SerpAPI** to perform real-time web searches
- 📝 Summarizes content with a **Langchain Summarization Chain**
- 📤 Sends output to a **Discord channel** via webhook
- 💬 Powered by **OpenAI GPT-4.1-mini**

---

## 🔧 Workflow Components

| Node                     | Description                                 |
|--------------------------|---------------------------------------------|
| `When chat message received` | Trigger node that starts on incoming message |
| `AI Agent`              | Langchain AI agent to handle task delegation |
| `OpenAI Chat Model`     | GPT-4.1-mini model to generate responses     |
| `SerpAPI`               | For real-time web search enrichment          |
| `Simple Memory`         | Stores context across sessions               |
| `Summarization Chain`   | Summarizes the final AI response             |
| `Discord`               | Sends final summary to Discord via webhook   |

---

## ⚙️ Requirements

- n8n (latest version recommended)
- OpenAI API Key
- Discord Webhook URL
- SerpAPI Key

---

## 🚀 How to Use

1. Clone this repository.
2. Import the workflow in your local or cloud **n8n** instance.
3. Set up credentials for:
   - OpenAI
   - Discord Webhook
   - SerpAPI
4. Activate the workflow.
5. Send a chat message — and see summarized replies posted on Discord!

---

## 📁 File Structure

