✨ The Muse – AI Creative Partner

A Multi-Agent System for Grounded Storytelling, Powered by Gemini

🎥 YOUTUBE VIDEO
## 🎥 Demo Video

[![Watch the video](https://img.youtube.com/vi/BgzJmZUsFJY/0.jpg)](https://youtu.be/BgzJmZUsFJY?si=mdt1Uzw67SYymDAF)


📖 Project Overview

Every writer knows the sting of the blank page — especially midway through a story.
You’ve built a world, shaped characters… and suddenly the path ahead goes dark.
Standard AI prompts often give clichés or break immersion with fake “facts.”

The Muse changes that.

This isn’t just a chatbot — it’s an
autonomous multi-agent creative partner
that thinks, researches, critiques, and writes with you.

💡 What Problem Does It Solve?

Writers get stuck because:

They don’t know what realistic event comes next

They want fresh, surprising plot twists

They can’t afford hallucinations or wrong facts

The Muse solves all three:

✔ Researches real-world context

✔ Generates grounded, creative twists

✔ Self-evaluates and filters low-quality ideas

🧠 System Architecture

The system is powered by three specialized agents:

🕵️‍♂️ 1. Researcher Agent – Grounding

Breaks down the story into keywords

Uses DuckDuckGo Search to find obscure facts

Provides real-world anchors for the plot

✍️ 2. Writer Agent – Creativity

Ingests story + research

Uses MemoryBank for user preferences

Produces three surprising, fact-based twists

⚖️ 3. Critic Agent – Evaluation

Grades each twist for:

Creativity

Factual grounding

Overall quality

Then provides:

A score

A short critique for each twist

🏛️ Core Concepts Implemented (5 Days of AI Course)
Concept	Implementation
Tool Use / Function Calling	Web search, name extraction
Sessions & Memory	MemoryBank storing user preferences
Observability	Custom AgentTracer logs every step
Self-Evaluation	Critic agent grading twist quality
Agent-to-Agent Communication	Data flow: Research → Write → Critic
Deployment	Gradio interactive app
🚀 Try It Yourself
1. Run All Cells

Installs dependencies and loads models.

2. Scroll to the Bottom

You’ll see the full Gradio UI, including:

Story input

Style selector

Generate button

Observability logs

3. Paste a Story Draft

Example starter:

“The year is 1854 in Soho, London…”

4. Click “Generate Twists”

Watch the agents research → write → critique in real time.

🛠️ Tech Stack

google-generativeai — Gemini 1.5 Flash & Pro

duckduckgo-search — Live factual grounding

gradio — Web interface

Python — Core logic

📦 Install Dependencies
pip install -q -U google-generativeai duckduckgo-search gradio

🔧 Setup Your API Key
import google.generativeai as genai
genai.configure(api_key="YOUR_API_KEY")

📝 Run the App
demo.launch(share=True)


This generates a temporary Gradio public link.

🌌 Features

✔ Multi-Agent Reasoning

✔ Research-driven plot twists

✔ Automatic twist scoring

✔ Real-time observability logs

✔ Clean UI for story testing

📈 Future Improvements

Replace MemoryBank with a vector database (Chroma / Pinecone)

Add access to specialized history/science databases

Human-in-the-loop twist scoring

Writer ↔ Critic debate for better refinement

💐 Conclusion

The Muse is a creative partner — part historian, part writer, part editor.
It blends imagination with real-world truth, crafting twists that feel lived-in and surprising.

A companion for every storyteller.
