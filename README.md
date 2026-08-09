<h2 align="center">Ирина Коршунова</h2>

<p align="center">
  <strong>Промпт-инженер | AI/ML Integration | Telegram Bots</strong>
</p>

<p align="center">
  <a href="https://t.me/i_Devos">
    <img alt="Telegram" src="https://img.shields.io/badge/Telegram-26A5E4?style=flat&logo=telegram&logoColor=white" height="28">
  </a>
  <a href="https://github.com/Ira-Korshunova?tab=repositories&sort=stargazers">
    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ira-Korshunova?style=flat&logo=github&logoColor=white&label=Stars&color=181717" height="28">
  </a>
  <a href="https://github.com/Ira-Korshunova?tab=followers">
    <img alt="GitHub followers" src="https://img.shields.io/github/followers/Ira-Korshunova?style=flat&logo=github&logoColor=white&label=Followers&color=181717" height="28">
  </a>
</p>

---

<h3 align="center">О себе</h3>

**Промпт-инженер и разработчик AI-решений.** Проектирую и внедряю ИИ-ассистентов для бизнеса: от промпта до продакшена. Превращаю языковые модели в надёжные рабочие инструменты — боты, RAG-системы, автоматизации процессов.

**Промпт-инжиниринг**
- Проектирование промптов под сложные сценарии: few-shot, chain-of-thought, структурированные JSON-форматы
- Оптимизация токенов и параметров генерации — качество ответов при меньших затратах на API
- RAG-системы: базы знаний, гибридный поиск (FAISS + BM25 + rerank), ассистенты с памятью
- Мультимодальные модели: текст, изображения (Qwen-VL), голос (Yandex SpeechKit)
- AI-assisted разработка: CLI-агенты (Claude Code), CLAUDE.md, Skills, MCP, мультиагентные команды (Claude Agents Team)

**Разработка и автоматизация**
- Веб-приложения и API: Python (Flask, FastAPI), JavaScript (vanilla JS), Jinja2
- Telegram/VK-боты с интеграцией нейросетей (OpenAI, DeepSeek, Qwen-VL, GigaChat, Yandex GPT)
- Автоматизация бизнес-процессов: n8n, API-интеграции, OCR (Tesseract)
- Деплой: Linux, Nginx, SSL, SSH, Docker, VPS

---

<h3 align="center">Избранные проекты</h3>

<table>
<tr>
<td>

<h4 align="center"><a href="https://github.com/Ira-Korshunova/porta-showcase">Porta · Vision &amp; Knowledge</a></h4>

<p align="center">
  <a href="https://porta.cygnusweb.ru">
    <img alt="Live demo" src="https://img.shields.io/badge/Demo-1e40af?style=flat&logo=data%3Aimage%2Fsvg%2Bxml%3Bbase64%2CPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iOC41IiBmaWxsPSJub25lIiBzdHJva2U9IiNmZmZmZmYiIHN0cm9rZS13aWR0aD0iMiIvPjxwYXRoIGQ9Ik0zLjUgMTJoMTdNMTIgMy41YzIuNiAyLjcgNCA1LjUgNCA4LjVzLTEuNCA1LjgtNCA4LjVjLTIuNi0yLjctNC01LjUtNC04LjVzMS40LTUuOCA0LTguNXoiIGZpbGw9Im5vbmUiIHN0cm9rZT0iI2ZmZmZmZiIgc3Ryb2tlLXdpZHRoPSIyIi8%2BPC9zdmc%2B&logoColor=white&labelColor=1e40af">
  </a>
</p>

**AI-ассистент для автоматизации импорта/экспорта — флагманский проект**

Веб-платформа для автоматизации рутины импортёров/экспортёров: извлечение данных из документов (B/L, инвойсы, договоры), распознавание товаров по фото, RAG-справочник по нормативной базе ВЭД, сверка факта поставки с договором, аналитика поставок. Flask-приложение с многостолбцовым AI-layout.

**Результат:** ручная обработка поставки сокращается с часов до минут. Разбор документов идёт программным OCR + regex-парсером без обращения к платным LLM-API — стоимость обработки рутинных документов близка к нулю.

<p align="center">
  <img alt="Porta — главная страница" src="https://raw.githubusercontent.com/Ira-Korshunova/porta-showcase/main/docs/screenshots/%D0%B3%D0%BB%D0%B0%D0%B2%D0%BD%D0%B0%D1%8F_%D1%81%D0%B2%D0%B5%D1%82%D0%BB%D0%B0%D1%8F.png" width="720">
</p>

**Stack:** Python, Flask, Jinja2, Vanilla JS, Chart.js, PDF.js, FAISS/BM25+RRF, SQLite/PostgreSQL+pgvector, Qwen-VL, Docker, Traefik

</td>
</tr>
<tr>
<td>

<h4 align="center"><a href="https://github.com/Ira-Korshunova/tg-vk-crosspost">tg-vk-crosspost</a></h4>
**Контент-фабрика кросс-постинга в Telegram и VK**

Система берёт ссылку на статью → генерирует пост (текст + картинка через Qwen/DashScope) → публикует **одновременно** в Telegram и ВКонтакте. Оркестратор на скиллах Claude Code + Python: таблица-очередь `queue.csv` как источник правды, двойной дедуп, ретрай без перегенерации, проверка токенов до постинга. VK — через VK ID OAuth 2.1 с PKCE и 3-шаговую загрузку фото.

**Результат:** один источник → готовые посты сразу в двух соцсетях без ручного копирования; двойной дедуп и ретраи без перегенерации не дублируют контент и не сжигают токены.

<p align="center">
  <img alt="Пост, опубликованный во ВКонтакте" src="https://raw.githubusercontent.com/Ira-Korshunova/tg-vk-crosspost/main/screenshots/08.png" width="330">
  <img alt="Тот же пост в Telegram" src="https://raw.githubusercontent.com/Ira-Korshunova/tg-vk-crosspost/main/screenshots/11_cropped.png" width="330">
</p>

**Stack:** Python, Claude Code Skills, Telegram Bot API, VK API (OAuth 2.1 PKCE), Qwen/DashScope

</td>
</tr>
<tr>
<td>

<h4 align="center"><a href="https://github.com/Ira-Korshunova/porta-rag-mcp">porta-rag-mcp</a></h4>
**RAG-база знаний как MCP-tools для AI-клиента**

MCP-сервер (FastMCP), выставляющий RAG-базу знаний (поиск по документам) как tools для любого AI-клиента — Claude Desktop, Cursor, ChatGPT. Оптимизация токенов: `search_knowledge_base` — retrieval **без LLM** (дёшево), `ask_knowledge_base` — полный RAG с генерацией. Demo-бэкенд TF-IDF (runnable без ключей) + интерфейс для production-движка FAISS + BM25 + rerank. Гибрид с Notion: оба сервера на одном Claude — «найди в базе и запиши в Notion».

**Результат:** поиск по базе знаний без вызова LLM — в разы дешевле полного RAG; одна и та же база подключается к любому AI-клиенту через стандартный протокол MCP.

**Stack:** Python, FastMCP (MCP), RAG, TF-IDF/numpy, FAISS (production)

</td>
</tr>
<tr>
<td>

<h4 align="center"><a href="https://github.com/Ira-Korshunova/work_bot">Work Bot</a></h4>
**Бот для обработки документов ВЭД**

Telegram-бот для работы с документами ВЭД: OCR-сканирование, анализ товаров, голосовые сообщения, запросы к нормативной базе через RAG (FAISS + BM25 + rerank).

**Результат:** документ → OCR → структура товаров и ответы по нормативной базе прямо в чате, включая голосовой ввод.

<p align="center">
  <img alt="Work Bot — диалог с ботом" src="https://raw.githubusercontent.com/Ira-Korshunova/work_bot/main/screens/dialog_import_docs_cropped.png" width="320">
</p>

**Stack:** Python, Tesseract OCR, FAISS, Yandex SpeechKit, Qwen-VL

</td>
</tr>
<tr>
<td>

<h4 align="center"><a href="https://github.com/Ira-Korshunova/vk-deepseek-bot">VK DeepSeek Bot</a></h4>
**VK-чат-бот с интеграцией DeepSeek**

Чат-бот ВКонтакте на базе DeepSeek. Память диалога (20 сообщений), интеграция через Long Poll API.

**Результат:** осмысленный диалог с памятью контекста — без переплаты за фреймворки, на чистом Long Poll API.

**Stack:** Python, VK API, DeepSeek

</td>
</tr>
</table>

---

<h3 align="center">Технический стек</h3>

<p align="center">
  <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white">
  <img alt="Flask" src="https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white">
  <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black">
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white">
  <img alt="OpenAI" src="https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white">
  <img alt="DeepSeek" src="https://img.shields.io/badge/DeepSeek-4D6BFE?style=flat&logo=deepseek&logoColor=white">
  <img alt="Qwen" src="https://img.shields.io/badge/Qwen-665CEE?style=flat&logo=qwen&logoColor=white">
  <img alt="Claude Code" src="https://img.shields.io/badge/Claude%20Code-D97757?style=flat&logo=anthropic&logoColor=white">
  <img alt="LangChain" src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white">
  <img alt="Ollama" src="https://img.shields.io/badge/Ollama-000000?style=flat&logo=ollama&logoColor=white">
  <img alt="n8n" src="https://img.shields.io/badge/n8n-EA4B71?style=flat&logo=n8n&logoColor=white">
  <img alt="Telegram" src="https://img.shields.io/badge/Telegram-26A5E4?style=flat&logo=telegram&logoColor=white">
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white">
</p>

---

<h3 align="center">Образование</h3>

| Программа | Институт | Год | Ключевые навыки |
|-----------|----------|-----|-----------------|
| [Практический курс по Claude Code](https://zerocoder.ru/course-claude-code) · [диплом (RU)](./certificates/zerocoder-claude-code-ru.png) · [диплом (EN)](./certificates/zerocoder-claude-code-en.png) | Zerocoder | 2026 | CLI, CLAUDE.md, Skills, MCP, мультиагентные системы, Docker, SSH/SSL, GitHub, локальные модели (Ollama), FastAPI, деплой |
| [Промпт-инжиниринг. Продвинутая программа](https://zerocoder.ru/prompt-engineer-with-ai-course) | Zerocoder | 2026 | Продвинутый промптинг, LangChain, LangFlow, fine-tuning LLM, no-code (n8n), векторные БД (RAG), мультимодальные модели, Cursor AI, Yandex Cloud, Google Cloud |

---

<h3 align="center">Контакты</h3>

<p align="center">
  <a href="mailto:irakorshunova@mail.ru">
    <img src="https://img.shields.io/badge/Email-D14836?style=flat&logo=gmail&logoColor=white" height="28">
  </a>
  <a href="https://t.me/i_Devos">
    <img src="https://img.shields.io/badge/Telegram-26A5E4?style=flat&logo=telegram&logoColor=white" height="28">
  </a>
  <a href="https://github.com/Ira-Korshunova">
    <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" height="28">
  </a>
</p>


