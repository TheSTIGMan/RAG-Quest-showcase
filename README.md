# Fun RAG

**[Play it live: https://fun-rag.duckdns.org/](https://fun-rag.duckdns.org/)**

AI chatbots are great at sounding confident, even when they're making things up. **Retrieval-Augmented Generation (RAG)** is how real companies fix that: the AI looks up answers in the company's own documents first, then answers only from what it found. Fun RAG is a browser game that teaches how RAG works, and how to keep it secure, through 11 short stages set around a pizza company called SliceCraft.

Each stage has a story, a lesson, a hands-on mini-game, a quiz and a short "explain it in your own words" step. Clear a stage to unlock the next house on the pizza-town map.

The game also ships with a **live RAG demo**: a real AI answering questions about a mock SliceCraft store handbook, showing every step of the pipeline and every security check along the way.

> Formerly called **RAG Quest**.

---

## Try it

| | |
|---|---|
| **The game** | https://fun-rag.duckdns.org/ (free, no account, no API key) |
| **The live demo** | https://fun-rag.duckdns.org/#demo |

The game runs entirely in your browser. The live demo is a public, **bring-your-own-key** app: you sign in and use your own OpenRouter key, so your questions are billed to you and never to the site owner. The demo shows an estimated cost for each model before you ask anything. Guest Customer questions are open to everyone; the Line Cook and Store Manager roles need an account.

---

## Features

- **11 hands-on stages**: hallucinations, the RAG pipeline, chunking, embeddings, vector search, safe prompt building, debugging bad answers, the 8 main attacks on RAG apps, spotting vulnerable code, defense in depth, and auditing AI-written code
- **Pixel-art pizza town**: a map where each stage is a house that unlocks as you progress, with XP, badges and ranks
- **Training Room and mini-games**: slice a handbook into chunks with live sliders, plot meanings on an embedding map, tune search cutoffs, and build an attack-proof pipeline
- **Boss-battle quizzes, teach-back and rewards**: prove you understood each stage, then open the reward chest
- **Code Quest**: short challenges about each stage's code. Fill the gap, put the lines in order, or find the bug
- **Live RAG demo**: ask a real AI as a guest, cook or manager, and watch the retrieved chunks and their scores, what your role hides, the exact prompt sent to the AI, and the cited answer
- **Pick your model**: Gemma 4 26B, Gemma 4 31B or Phi-4, with the tokens used and the cost OpenRouter reported shown after each answer
- **Policy documents tab**: read the handbook yourself and check the AI's answers against it
- **See how the code works**: follow your question through the pipeline's Python code stage by stage, with a plain-English explanation on every line. The code is simplified, and security-sensitive details are left out on purpose
- **Security built in and shown**: input validation, a prompt-injection filter, role-based access control, a relevance cutoff, a poisoned-document quarantine, and a check that the AI's answer really cites what it retrieved, each shown passing or blocking in real time
- **Safe public accounts**: passwords are hashed, API keys are stored encrypted, can be deleted at any time, and are never shown back to the browser, and the demo has rate limits to stop abuse
- **Glossary, Cheat Sheet and Review mode**: look things up, download a one-page security cheat sheet, or replay finished stages
- **Explain Like I'm 5 mode** switches every lesson to simple, kid-friendly wording
- **Progress saved only in your browser**: no tracking
- **Accessible**: full keyboard support, screen-reader labels, and respects "reduce motion"

---

## Tech Stack

![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-strict-3178C6?logo=typescript&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-build-646CFF?logo=vite&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4-06B6D4?logo=tailwindcss&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.11%2B-3776AB?logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-backend-009688?logo=fastapi&logoColor=white)
![ChromaDB](https://img.shields.io/badge/ChromaDB-vector%20DB-orange)
![SQLite](https://img.shields.io/badge/SQLite-accounts-003B57?logo=sqlite&logoColor=white)
![OpenRouter](https://img.shields.io/badge/OpenRouter-Gemma%204%20%7C%20Phi--4-6B4FBB)
![Docker](https://img.shields.io/badge/Docker-deployed-2496ED?logo=docker&logoColor=white)
![Traefik](https://img.shields.io/badge/Traefik-HTTPS-24A1C1?logo=traefikproxy&logoColor=white)
![Security](https://img.shields.io/badge/Security-injection%20filter%20%2B%20RBAC-red)

---

## Screenshots

**Pizza town.** Every stage is a house on the map. The next one to play is featured up top.

![Home screen with the pizza-town map](screenshots/01-home.png)

**The live RAG demo.** Pick a role and a model, then try a suggested question (including a prompt-injection attack and a poisoned document) or ask your own.

![Live demo chat page with role picker and suggested questions](screenshots/02-live-demo.png)

---

## Source Code

The full source code for this project is maintained in a private repository. This showcase is for demonstration purposes only.

Built by [@TheSTIGMan](https://github.com/TheSTIGMan).
