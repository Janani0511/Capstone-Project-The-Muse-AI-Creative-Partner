The Muse – AI Creative Partner

A Multi-Agent System for Grounded Storytelling, Powered by Gemini

📖 Project Overview

Every writer knows the sting of the blank page, especially midway through a story. You’ve built a world, shaped characters… and suddenly the path ahead goes dark. Standard AI prompts often spit out clichés or break immersion with fake “facts.”

The Muse aims to change that.

This isn’t just a chatbot.
This is an autonomous multi-agent creative partner that thinks, researches, critiques, and writes like a collaborator who brings both imagination and real-world grounding.

💡 What Problem Does It Solve?

Fiction writers often get stuck because:

They don’t know what realistic event can happen next.

They want a twist that surprises, not something generic.

They can’t afford hallucinations that break historical or scientific believability.

The Muse solves all three:

It researches real facts.

It generates twists based on your story + real context.

It self-evaluates and filters bad ideas before you ever see them.

🧠 System Architecture

The system is powered by three specialized AI agents:

🕵️‍♂️ 1. Researcher Agent – Grounding

Breaks down the story into keywords.

Uses DuckDuckGo Search (via duckduckgo-search) to gather obscure factual context.

Returns real-world anchors the story can build upon.

✍️ 2. Writer Agent – Creativity

Ingests the story + research.

Reads user writing style + long-term preferences from a MemoryBank.

Produces three original, surprising, fact-based plot twists.

⚖️ 3. Critic Agent – Evaluation

Grades each twist for:

Creativity

Use of real facts

Overall quality

Provides a score and mini-review for every twist.

🏛️ Core Concepts Implemented (From “5 Days of AI” Course)
Concept	Implementation
Tool Use / Function Calling	Web search, name extraction
Sessions & Memory	User preferences stored in a MemoryBank
Observability	Custom AgentTracer logs every step
Self-Evaluation	Critic agent grades twist quality
Agent-to-Agent Communication	Writer uses Researcher + Memory output
Deployment	Gradio-based interactive interface
🚀 Try It Yourself
1. Run All Cells

The notebook installs dependencies and loads models.

2. Scroll to the Bottom

You’ll see the full Gradio UI with:

Story input

Style selector

“Generate Twists” button

Agent logs panel (live trace)

3. Paste Your Story Draft

Example starter:

The year is 1854 in Soho, London…

4. Hit “Generate Twists”

Watch the agents research, write, critique — all in real time.

🛠️ Tech Stack

google-generativeai — Gemini 1.5 Flash & Pro

duckduckgo-search — Live factual grounding

gradio — Web UI

Python — Orchestration and logic

📦 Install Dependencies
pip install -q -U google-generativeai duckduckgo-search gradio

🔧 Setup Your API Key
import google.generativeai as genai
genai.configure(api_key="YOUR_API_KEY")

📝 Running the App
demo.launch(share=True)


This generates a temporary public URL via Gradio.

🌌 Features
✔ Multi-Agent Reasoning

Each agent is specialized, making the system more reliable than a single prompt.

✔ Research-Driven Plot Twists

No hallucinations. Twists come from real facts.

✔ Self-Evaluation via Critic Agent

Bad twists get filtered out before reaching you.

✔ Live Observability Logs

Watch the "thinking" and tool usage as it happens.

✔ Interactive UI

Clean Gradio interface for writers of any skill level.

📈 Future Improvements

Replace MemoryBank with a real vector database (ChromaDB / Pinecone)

Give the Researcher access to specialized historical/scientific datasets

Let users upvote/downvote twist quality (human-in-the-loop)

Add iterative debate between Writer ↔ Critic for better twist refinement

💐 Conclusion

The Muse is a glimpse into the future of creative tools — part historian, part writer, part editor.
It blends imagination with truth, crafting twists that feel lived-in, unpredictable, and grounded.

A companion for every storyteller.
