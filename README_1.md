# AI Agents & Automation with n8n

A self-paced course website covering 77 lessons across 7 modules: AI agent fundamentals, your first agent, RAG agents, n8n triggers and nodes, and business AI agents. Each lesson includes reference videos, a hands-on build, and links to the n8n docs.

It's one file (`index.html`) with no build step. Progress and notes are saved in each visitor's own browser.

## Publish on GitHub Pages

1. Create a new public repository on GitHub, for example `n8n-course`.
2. Click **Add file → Upload files**, drag in `index.html` and `README.md`, and click **Commit changes**.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose the `main` branch and the `/ (root)` folder, then click **Save**.
5. Wait a minute or two. Your site will be live at `https://<your-username>.github.io/n8n-course/`.

## Edit the course

All lesson content is in the `COURSE` list inside the `<script>` at the bottom of `index.html`. Each lesson has this shape:

```
["Title", "m:ss" or null, "Summary", ["What you'll learn"], ["Practice steps"], "YouTube search phrase", ["docs keys"], ["official video keys"]]
```

To link a specific video, add it to the `OFFICIAL` list and reference its key in the lesson.

Direct links to a lesson use its ID, for example `.../n8n-course/#m3l5` opens Module 3, Lesson 5.
