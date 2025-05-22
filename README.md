# 🧠 **Todo Summary Assistant**

*Your AI-powered task manager with smart summaries & Slack sync*

Manage your tasks like a pro with AI-powered insights! With Todo Summary Assistant, you can create, update, complete tasks — and with one click, generate a friendly summary of your pending todos using **GPT-4o-mini**. Bonus? That summary is automatically sent to your **Slack team**. 🎯

---

## 🌍 **Live Demo**

🔗 [Check it out here](https://todo-summary-assistant-five.vercel.app/)

---

## 🧩 **Project Structure**

```
📁 Frontend/  →  React app with all components, Tailwind UI, and API hooks  
📁 Backend/   →  Node.js server, API routes, OpenAI & Slack integrations
```

---

## 🏗️ **Architecture Overview**

Here’s how all parts of the system come together:

![architecture-diagram](https://github.com/user-attachments/assets/ff044c37-6962-49dd-8988-6bbdcfdb71ac)



---

## 🖼️ **Frontend Setup (React + Vite)**

### 🚀 Get Started

```bash
cd Frontend
npm install
npm run dev
```

### 🔐 Add Environment Variables

Create a `.env` file inside `Frontend/` with:

```env
VITE_API_BASE_URL=https://todo-summary-assistant-1x1s.onrender.com
```

> Replace the URL if you're running the backend locally or on another server.

---

## 🛠️ **Backend Setup (Node.js + Express)**

### 🚀 Start the Server

```bash
cd Backend
npm install
npm start
```

✅ Ensure your **Supabase database** is correctly configured.

### 🔐 Add Environment Variables

Create a `.env` file inside `Backend/` with:

```env
PORT=5000
DATABASE_URL=your_supabase_postgres_connection_string
OPENAI_API_KEY=your_openai_api_key
SLACK_WEBHOOK_URL=your_slack_webhook_url
```

* `DATABASE_URL` → from your Supabase project
* `OPENAI_API_KEY` → from your OpenAI account
* `SLACK_WEBHOOK_URL` → from Slack > Apps > Incoming Webhooks

---

## ✨ **Key Features**

* 📝 **Create, update, and delete todos**
* ✅ **Mark tasks as complete**
* 🧠 **Get instant summaries powered by GPT-4o-mini**
* 📤 **Auto-send summaries to your Slack workspace**
* 💻 **Built with React + Tailwind CSS for sleek UI**
* 🌐 **API-powered backend with Node.js**
* 🗃️ **Supabase PostgreSQL for persistent storage**

---

## 🧠 **AI-Powered Prompt Logic**

Our smart summarizer uses GPT-4o-mini with a tailored prompt to:

* 🔄 Reword tasks into a concise, natural paragraph
* 🚫 Avoid bullet points or numbering
* 🎯 Highlight task importance and urgency
* 💬 Use a friendly, conversational tone ideal for Slack updates

---

## 🛠️ Tech Stack

* **Frontend:** React, Vite, Tailwind CSS
* **Backend:** Node.js, Express
* **Database:** Supabase (PostgreSQL)
* **AI:** OpenAI GPT-4o-mini
* **Integration:** Slack Webhooks
