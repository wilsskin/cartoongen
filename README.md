# CartoonGen
Generate satirical political cartoons from today's top headlines.

[cartoongen-ai.vercel.app](https://cartoongen-ai.vercel.app)

**Team:** [Wilson Skinner](https://github.com/wilsskin), [Aryan Dagnas](https://github.com/aryandaga7)

---

## What It Does
- Pulls the top three headlines from five major news outlets each morning
- Lets users generate a satirical cartoon from any headline with one click
- Returns a downloadable, shareable image

## How It's Built
React and Vite frontend backed by a FastAPI Python API. Each morning a Vercel Cron job runs a Python script that fetches RSS feeds from five outlets and stores headlines in a Neon Postgres database. The site only shows today's results. When a user selects a headline, the app builds a prompt and calls the Gemini API to generate the cartoon.

**Stack:** React, Vite, FastAPI, Neon Postgres, Gemini API, Vercel
