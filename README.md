# AI-Powered GeoExplorer: Adaptive Web Quizzes with ArcGIS

Demos and materials from my talk  
**“AI-Powered GeoExplorer: Adaptive Web Quizzes with ArcGIS”**  

This repo shows how to combine:

- ArcGIS Maps SDK for JavaScript  
- Generative AI (OpenAI, Gemini) along with TensorFlow.js and Azure Sentiment Analysis  
- Light gamification patterns (quizzes, difficulty, feedback)

to turn web maps into adaptive learning experiences.

---

## Contents

- `demo1-starter-code.html`  
  Starter file for the **AI Question Map** live coding segment.  
  Minimal wiring is in place so you can follow along and finish the prompt and API call yourself.

- `demo1-github.html`  
  Completed version of **Demo 1 – AI Question Map**.  
  Click the map, send coordinates to an LLM, and show a short question and answer about that spot.

- `demo2-github.html`  
  Completed version of **Demo 2 – Gemini + ArcGIS countries**.  
  Type a natural language description and let Gemini return country names that drive a FeatureLayer query.

- `demo3-github.html`  
  Completed version of **Demo 3 – GeoExplorer**.  
  An end to end quiz loop:
  - Click a location to start a round  
  - Use ArcGIS geocoding for local context  
  - Generate multiple choice questions with an LLM  
  - Adjust difficulty over time  
  - Capture sentiment and a short “vibe recap” of the map session

---

## Running the demos

These files are plain HTML and JavaScript. You have two easy options:

1. **Open directly in a browser**

   - Download or clone this repo.
   - Open any `demo*.html` file in a modern browser (Chrome, Edge, Firefox).

2. **Serve with a simple local web server** (recommended)

   This avoids CORS issues and matches how you would host these in practice.

   Example with `npx`:

   ```bash
   npx serve .
