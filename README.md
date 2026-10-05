# RAG Quest

AI chatbots are great at sounding confident, even when they're making things up. **Retrieval-Augmented Generation (RAG)** is how real companies fix that: the AI looks up answers in the company's own documents first, then answers only from what it found. RAG Quest is a browser game that teaches how RAG works, and how to keep it secure, through 11 short levels set in the kitchen of a pizza company called SliceCraft.

Each level is an order ticket on the kitchen's ticket rail. You read the story, learn the idea, play a hands-on mini-game, take a quiz, and explain it back in your own words. Finished orders get stamped **SERVED**.

The game also ships with a **live RAG demo**: a real AI answering questions about a mock SliceCraft store handbook, showing every step of the pipeline and every security check along the way.

---

## Features

- **11 hands-on levels**: hallucinations, the RAG pipeline, chunking, embeddings, vector search, safe prompt building, debugging bad answers, the 8 main attacks on RAG apps, spotting vulnerable code, defense in depth, and auditing AI-written code
- **Interactive mini-games**: slice a handbook into chunks with live sliders, plot meanings on an embedding map, tune search cutoffs, and build an attack-proof pipeline
- **Live RAG demo**: ask a real AI as a guest, cook or manager, and watch the retrieved chunks and their scores, what your role hides, the exact prompt sent to the AI, and the cited answer
- **Security built in and shown**: input validation, a prompt-injection filter, role-based access control, a relevance cutoff, and a poisoned-document quarantine, each shown passing or blocking in real time
- **Explain Like I'm 5 mode** switches every lesson to simple, kid-friendly wording
- **Progress, XP, badges and ranks** saved only in your browser: no account, no tracking
- **Downloadable security cheat sheet** covering the whole pipeline on one page
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
![OpenRouter](https://img.shields.io/badge/OpenRouter-Gemma%204-6B4FBB)
![Security](https://img.shields.io/badge/Security-injection%20filter%20%2B%20RBAC-red)

---

## Screenshots

**The ticket rail.** Every level is an order ticket. The next one to play is featured up top.

![Home screen with the featured ticket](screenshots/01-home.png)

![The ticket rail with served, current and locked levels](screenshots/02-ticket-rail.png)

**Inside a level.** A story told through kitchen chat, then hands-on mini-games like the chunking lab.

![Story step for the Embeddings level](screenshots/03-story.png)

![The Goldilocks chunking lab mini-game](screenshots/04-minigame.png)

**The live RAG demo.** A real AI answer, grounded in the handbook with citations, next to each pipeline step.

![Live demo answering a refund question with citations](screenshots/05-live-demo.png)

**Security in action.** A prompt-injection attempt is stopped at the input filter, before anything is retrieved or the AI is ever called.

![Prompt injection attempt blocked](screenshots/06-injection-blocked.png)

**Finish all 11 levels** and the final receipt comes out stamped.

![RAG Hero completion screen](screenshots/07-rag-hero.png)

**Works on phones too.**

<img src="screenshots/08-mobile.png" alt="RAG Quest on a phone" width="320">

---

## Source Code

The full source code for this project is maintained in a private repository. This showcase is for demonstration purposes only.

Built by [@TheSTIGMan](https://github.com/TheSTIGMan).
