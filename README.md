# PROMPT·LAB — Electro-Biomorph Prompt Evaluation Studio

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/YOUR_USERNAME/prompt-lab/blob/main/Prompt_Studio_Biomorph.ipynb)

Write a prompt, get it scored by an AI judge on six pillars, then watch it evolve.
Runs entirely in Google Colab (Python + Flask + vanilla HTML/JS). No Streamlit.

![Hero](assets/hero.png)
![Dashboard](assets/dashboard.png)

## What it does
- **LLM-as-a-judge** scoring across Role, Goal, Context, Constraints, Format and Style (0–10 each, overall /100 calculated in Python)
- **Structured output**: strict JSON schema on gpt-oss models, with an automatic plain-JSON fallback for other models
- **Radar chart** that overlays your previous attempt, animated gauge, expandable per-criterion feedback
- **Optimized prompt** with copy / use-in-editor / re-evaluate
- **Battle test**: run your prompt and the optimized one side by side
- **Improvement journey**: score chart + attempt history, click to restore any version
- **Live quick-scan** of the six pillars while you type (instant, client-side heuristics)
- **Challenge picker**: 5 domains x 3 difficulty levels
- **Export** a Markdown report or JSON history

## UI / motion
- Spring-physics smooth caret in the prompt box
- Scroll-driven kinetic typography and converging pillar icons
- Cursor-reactive letters, text-scramble labels
- Direct-follow dot vs spring-follow orb
- Clip-path "reel" popover with custom media controls (canvas-generated, no video file)
- Live "dial" panel to tune spring stiffness, damping, mass, glow and font size
- Charcoal black / forest green / crimson electro-biomorph theme

## Run it
1. Get a free API key at <https://console.groq.com/keys>
2. Click the **Open in Colab** badge above (or upload `Prompt_Studio_Biomorph.ipynb` to Colab)
3. Run **cell 1** and paste your key when asked (it is never stored in the notebook)
4. Run **cell 2**; click **OPEN PROMPT·LAB IN A NEW TAB** (or use the inline copy)

> The link comes from Colab's port proxy: it only works while the runtime is running, and only for the Google account that owns the notebook.

## Tech
Python · Flask · Groq API (`openai/gpt-oss-20b`, `openai/gpt-oss-120b`, `llama-3.3-70b-versatile`) · hand-rolled SVG/canvas charts · Web Animations API

## Credits
Motion ideas inspired by [Skiper UI](https://skiper-ui.com) (gxuri). Re-implemented in vanilla JS.

## License
MIT
