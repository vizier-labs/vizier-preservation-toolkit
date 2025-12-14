# Vizier Preservation Toolkit (v1.0)

The Vizier Preservation Toolkit is a browser-local system for managing multi-session AI work.

It helps preserve context, decisions, and artifacts so work can be reliably continued across sessions and across different AI models.

The toolkit separates three concerns that are often mixed together in AI workflows:

- **State** – what has been completed, decided, and validated
- **Artifacts** – drafts, code, notes, and extracted outputs
- **Restoration** – clear instructions that allow an AI to resume work correctly

All data is stored locally in your browser.  
Nothing is transmitted, synced, or logged externally.

The toolkit is model-agnostic and works equally well with ChatGPT, Claude, and other LLMs.  
It is intentionally implemented as a single HTML file so it can be inspected, archived, and used offline.

This tool does not replace prompts or documents.  
It provides structure so those things remain usable over time.

This project accompanies the [Vizier Beginner Guide](https://archive.org/details/viziers-beginner-guide-to-ai-projects-120725) and the Vizier Advanced Guide.

---

## What This Is Not

- Not a SaaS product  
- Not a backend service  
- Not an AI wrapper or agent framework  
- Not a collaboration platform  

There are no accounts, no servers, no tracking, and no telemetry.

---

## Core Concepts

### Projects
A project represents a coherent body of work. All checkpoints, work logs, and artifacts belong to a project.

### Checkpoints (State Ledger)
Durable snapshots of progress. Checkpoints are designed to be restoration points and typically record:

- What was completed
- Key decisions
- Files or artifacts involved
- What comes next

### Work Logs
Lightweight records of progress between checkpoints. Work logs document work without creating a new restoration boundary.

### Artifacts (Artifact Registry)
Extracted outputs such as drafts, code, diagrams, notes, or references that should persist independently of chat history.

### Restoration Prompt Generator
Produces a clean, structured prompt that allows an AI to resume work correctly using saved state and artifacts.

---

## Using the Toolkit

### Web Version (Instant Access)
Use the toolkit directly in your browser — no download required:

**https://vizier-labs.github.io/vizier-preservation-toolkit/**

### Download for Offline Use
Download [vizier-preservation-toolkit-v1.0.html](https://github.com/vizier-labs/vizier-preservation-toolkit/blob/main/vizier-preservation-toolkit-v1.0.html) and open it in any modern browser.

No installation  
No backend  
No extensions  
Your data stays local

---

## Recommended Workflow

1. **Start a project cleanly**
2. **Open a session by stating:**
   - what you are doing  
   - what you already have  
   - what help you want  
3. **Save checkpoints when progress is real**
4. **Use the toolkit’s checkpoint generator to capture:**
   - completed work  
   - decisions  
   - files  

### Next Steps
Use work logs between checkpoints to record progress without creating unnecessary restoration points.

### Restore When Needed
Upload artifacts, paste your last checkpoint, and use the restoration prompt to continue work accurately.

---

## Documentation

- [Vizier Beginner Guide](https://archive.org/details/viziers-beginner-guide-to-ai-projects-120725)  
  A practical introduction to structured AI work (~18,000 words)

- [Vizier Advanced Guide](https://archive.org/details/viziers-guide-managing-artificial-intelligences-120725)  
  A deep technical and methodological reference (~102,000 words)

- Quick Start Card  
  One-page workflow reference for daily use

---

## Privacy Model

- All data is stored in browser local storage  
- No external requests  
- No analytics  
- No cookies beyond local persistence  

You can inspect the full source by opening the HTML file in any text editor.

---

## License

This work is licensed under **Creative Commons Attribution–NonCommercial–ShareAlike 4.0 (CC BY-NC-SA 4.0)**.

See `NOTICE.md` for full terms.
