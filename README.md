https://bhavyarana1909-collab.github.io/fakenews-detection-ml/
# KhabarCheck 📰🔍

A premium, browser-based Fake News Detection dashboard. KhabarCheck features a dual-engine architecture, combining an advanced offline NLP heuristic scorer with live LLM integration via OpenRouter for high-accuracy analysis.

## ✨ Key Features
* **Dual Analysis Engine:** 
  * **Offline Mode:** Uses a Weighted Lexicon Scoring Algorithm to detect sensationalism, clickbait, and conspiracy markers without internet.
  * **Online Mode:** Connects to OpenRouter API (Gemini/Claude/GPT) for deep contextual LLM analysis.
* **Media Support:** Analyze raw text or upload images (with simulated OCR processing UI).
* **Premium UI:** Light-mode glassmorphic design built with Tailwind CSS.
* **Zero Backend:** 100% client-side processing. No server required.

## 🛠️ Tech Stack
* **Frontend:** HTML5, Vanilla JavaScript, Tailwind CSS (CDN)
* **Visualizations:** Chart.js
* **API Integration:** OpenRouter

## 🚀 How to Run
1. **Download/Clone:** Download the repository to your local machine.
2. **Open:** Double-click `index.html` to open it in any modern web browser.
3. **Analyze:** Paste news text or upload an image.
4. **(Optional) API Key:** Paste your OpenRouter API key into the header input to unlock the live LLM-powered engine. If left blank, the app seamlessly uses the offline heuristics engine.

## 🧠 How the Offline Engine Works
The built-in offline engine analyzes text across multiple dimensions:
* **Credibility Markers:** Reduces fake probability if professional journalistic attribution ("according to", "reported by") is found.
* **Categorized Suspicion:** Heavily penalizes conspiracy terms while moderately penalizing clickbait/urgent formatting.
* **Ratio Math:** Normalizes scores based on word count to prevent false positives on long, legitimate articles.

---
*Built for a clean, fast, and accurate fact-checking experience.*
