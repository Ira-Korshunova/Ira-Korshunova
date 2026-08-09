<h1 align="center">Ирина Коршунова</h1>

<p align="center">
  <strong>Python Developer | AI/ML Integration | Telegram Bots</strong>
</p>

<p align="center">
  <a href="https://github.com/Ira-Korshunova?tab=repositories&sort=stargazers">
    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ira-Korshunova?style=social">
  </a>
  <a href="https://github.com/Ira-Korshunova?tab=followers">
    <img alt="GitHub followers" src="https://img.shields.io/github/followers/Ira-Korshunova?style=social">
  </a>
</p>

---

## О себе

Разработчик AI-ботов и систем автоматизации. Специализируюсь на AI-assisted development с Claude Code, продвинутом промптинге, создании Telegram-ботов с интеграцией нейросетей, RAG-систем для работы с документами и автоматизации бизнес-процессов через no-code (n8n) и API.

**Фокус:**
- **Claude Code / AI-assisted development** — CLI-агенты, CLAUDE.md, Skills, MCP, мультиагентные системы (Claude Agents Team), деплой (SSH/SSL, Docker, VPS)
- **Промпт-инжиниринг** — few-shot, chain-of-thought, структурированные форматы (JSON), RAG (базы знаний, FAISS + BM25 + rerank), LangChain/LangFlow
- **Python-разработка** — Flask, FastAPI, Telegram/VK-боты, интеграции нейросетей (OpenAI, DeepSeek, Qwen-VL, GigaChat, Yandex GPT)
- **Автоматизация бизнес-процессов** — n8n, API-интеграции, no-code связки, OCR (Tesseract), голосовые интерфейсы (Yandex SpeechKit)

> Выпускница Zerocoder по направлению «Промпт-инжиниринг. Продвинутая программа» и курсу «Практический курс по Claude Code» (см. блок «Образование»).

---

## Технический стек

| Категория | Технологии |
|-----------|------------|
| **Языки** | Python 3.10+, SQL |
| **Фреймворки** | Flask, asyncio, Jinja2, FastAPI |
| **AI/ML** | OpenAI, DeepSeek, Qwen-VL, Gemini, Gigachat, Yandex GPT |
| **AI-агенты** | Claude Code (CLI), CLAUDE.md, Skills, MCP |
| **Мультиагентность** | Claude Agents Team, LangChain, LangFlow |
| **Промптинг** | few-shot, chain-of-thought, JSON-форматы |
| **Базы данных** | PostgreSQL, SQLite, FAISS, векторные хранилища (RAG) |
| **No-code** | n8n, EMD Cloud, Albato |
| **Инструменты** | Docker, Git, Tesseract OCR, Ollama (локальные модели) |
| **Деплой** | Linux, Nginx, SSL, SSH, systemd, VPS |
| **Облака** | Yandex Cloud, Google Cloud |
| **API** | Telegram Bot API, VK, Google Sheets, WhatsApp |

---

## Образование

| Программа | Институт | Год | Ключевые навыки |
|-----------|----------|-----|-----------------|
| [Практический курс по Claude Code](https://zerocoder.ru/course-claude-code) | Zerocoder | 2025 | CLI, CLAUDE.md, Skills, MCP, мультиагентные системы, Docker, SSH/SSL, GitHub, локальные модели (Ollama), FastAPI, деплой |
| [Промпт-инжиниринг. Продвинутая программа](https://zerocoder.ru/prompt-engineer-with-ai-course) | Zerocoder | 2025 | Продвинутый промптинг, LangChain, LangFlow, fine-tuning LLM, no-code (n8n, EMD Cloud), векторные БД (RAG), мультимодальные модели, Cursor AI, Yandex Cloud, Google Cloud |

---

## Избранные проекты

<table>
<tr>
<td>

### [Porta](https://github.com/Ira-Korshunova/porta-showcase) · [🟢 live demo](https://porta.cygnusweb.ru)
**AI assistant for import/export automation — флагманский проект**

Веб-платформа для автоматизации рутины импортёров/экспортёров: извлечение данных из документов (B/L, инвойсы, договоры), распознавание товаров по фото, RAG-справочник по нормативной базе ВЭД, сверка факта поставки с договором, аналитика поставок. Flask-приложение с многостолбцовым AI-layout.

**Stack:** Python, Flask, Jinja2, Vanilla JS, Chart.js, PDF.js, FAISS/BM25+RRF, SQLite/PostgreSQL+pgvector, Qwen-VL, Docker, Traefik

</td>
</tr>
<tr>
<td>

### [tg-vk-crosspost](https://github.com/Ira-Korshunova/tg-vk-crosspost)
**Контент-фабрика кросс-постинга в Telegram и VK**

Система берёт ссылку на статью → генерирует пост (текст + картинка через Qwen/DashScope) → публикует **одновременно** в Telegram и ВКонтакте. Оркестратор на скиллах Claude Code + Python: таблица-очередь `queue.csv` как источник правды, двойной дедуп, ретрай без перегенерации, проверка токенов до постинга. VK — через VK ID OAuth 2.1 с PKCE и 3-шаговую загрузку фото.

**Stack:** Python, Claude Code Skills, Telegram Bot API, VK API (OAuth 2.1 PKCE), Qwen/DashScope

</td>
</tr>
<tr>
<td>

### [porta-rag-mcp](https://github.com/Ira-Korshunova/porta-rag-mcp)
**RAG knowledge base как MCP-tools для AI-клиента**

MCP-сервер (FastMCP), выставляющий RAG-базу знаний (поиск по документам) как tools для любого AI-клиента — Claude Desktop, Cursor, ChatGPT. Оптимизация токенов: `search_knowledge_base` — retrieval **без LLM** (дёшево), `ask_knowledge_base` — полный RAG с генерацией. Demo-бэкенд TF-IDF (runnable без ключей) + интерфейс для production-движка FAISS + BM25 + rerank. Гибрид с Notion: оба сервера на одном Claude — «найди в базе и запиши в Notion».

**Stack:** Python, FastMCP (MCP), RAG, TF-IDF/numpy, FAISS (production)

</td>
</tr>
<tr>
<td width="50%">

### [Work Bot](https://github.com/Ira-Korshunova/work_bot)
**Document processing bot for foreign trade**

Telegram-бот для работы с документами ВЭД: OCR-сканирование, анализ товаров, голосовые сообщения, запросы к нормативной базе через RAG (FAISS + BM25 + rerank).

**Stack:** Python, Tesseract OCR, FAISS, Yandex SpeechKit, Qwen-VL

</td>
<td width="50%">

### [VK DeepSeek Bot](https://github.com/Ira-Korshunova/vk-deepseek-bot)
**VK chatbot with DeepSeek integration**

Чат-бот ВКонтакте на базе DeepSeek. Память диалога (20 сообщений), интеграция через Long Poll API.

**Stack:** Python, VK API, DeepSeek

</td>
</tr>
</table>

---

## GitHub Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Ira-Korshunova&show_icons=true&theme=dark&hide_border=true" height="170">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ira-Korshunova&layout=compact&theme=dark&hide_border=true&langs_count=6" height="170">
</p>

---

## Contact

<p align="center">
  <a href="mailto:irakorshunova@mail.ru">
    <img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white">
  </a>
  <a href="https://github.com/Ira-Korshunova">
    <img src="https://img.shields.io/badge/GitHub-100000?style=flat&logo=github&logoColor=white">
  </a>
</p>

<p align="center">
  <em>Open to freelance projects and collaboration</em>
</p>
