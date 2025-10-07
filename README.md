Smart Study — Single-file Revision Helper

Overview

Smart Study is a single-page responsive web app (single HTML file) built with plain HTML, CSS, and JavaScript. It helps school students revise from coursebook PDFs using a set of mock AI features, a quiz generator, and a progress tracker that stores results in the browser's localStorage.

Files

- `smart-study.html` — The entire app (HTML, internal CSS, and JS). Open this in your browser to run the app.

How to run

1. Open the workspace folder in your file explorer or VS Code.
2. Double-click `smart-study.html` or right-click -> Open With -> your browser.
3. The app runs fully client-side; no server is required.

Features (short)

- Navbar & Menu — Animated top navigation with a hamburger toggle. Menu items smoothly scroll to page sections.
- PDF Selector — Upload your own PDF or choose from small preloaded samples (place sample PDFs alongside the HTML file).
- PDF Viewer — Embedded viewer using `<embed>` to preview the selected PDF inside the app.
- Quiz Generator — Creates mock MCQs, short-answer, and long-answer prompts. Basic grading and immediate feedback.
- Progress Tracker — Saves quiz attempts in `localStorage` and shows a mini-dashboard (count, average, last score).
- AI Chat (Virtual Teacher) — Offline mock chat that provides short answers with citation snippets and page numbers.
- Cited Answers — Historical list of cited snippets returned by the chat for quick review.
- YouTube Recommender — Suggests topic-related videos (links open in a new tab).

More details about each feature are described above in the Features section.

Design & Theme

- Theme uses only yellow and green shades (no white/black). Cards have 15px borders and padding as requested.
- Mobile responsive: grid collapses to single column on small screens. Toggle menu and chat scale down responsively.
- Smooth scrolling, subtle animations, typing indicator, section reveal on scroll.

Limitations & Notes

- The AI is mocked for offline use. To use a real LLM API, you must add API calls (server-side is recommended to keep API keys secret).
- Cited answers are mocked. For real citations, extract text from PDFs (e.g., using pdf.js), find relevant passages, and then either present quotes or feed them to an LLM.
- `sample1.pdf`, `sample2.pdf`, and `sample3.pdf` are referenced as example preloaded files. If you want preloaded PDFs, add them to the same folder as `smart-study.html`.

Next steps (optional)

- Integrate `pdf.js` to extract text so citations are accurate.
- Hook up an LLM (OpenAI, etc.) with server-side proxy to provide real AI answers and better question understanding.
- Improve accessibility (ARIA attributes, keyboard navigation for menu items and quiz controls).
- Add persistence for uploaded PDF selection (e.g., store last-used filename in localStorage).

Contact / Help

If you'd like, I can:

- Bundle 1–2 sample PDFs into the folder.
- Add pdf.js client-side extraction and make citations real.
- Show how to wire an LLM API securely using a small server example.

Open an issue or tell me which next step you want and I'll implement it.
