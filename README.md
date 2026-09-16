# Nathan Mathew

**AI Engineer focused on agents that check their own work.**

I build systems that don't just call an LLM and return whatever comes back — they validate the output against a real specification, catch their own mistakes, and either fix them or say so. My invoice-extraction agent ([INTAKE-AGENT](https://github.com/nathanmathew24/INTAKE-AGENT)) is the clearest example: it retries against structured validation errors, and its README documents a failure mode it has — where the retry loop can "fix" a document by rewriting the wrong field — rather than hiding it. I'd rather ship something with a documented limitation than something that looks finished and isn't.

I work mainly in Python, with FastAPI/Streamlit for interfaces, Pydantic for schema validation, and LLM APIs (OpenAI, Groq) for the parts that need language understanding rather than rules. I've also shipped full-stack TypeScript/React work (Next.js + Supabase, React + FastAPI).

---

## What I build

- **Document & data extraction agents** — turning unstructured input (PDFs, images, forms) into validated, typed records, with retry logic against real constraints rather than a single best-effort pass.
- **Multi-agent pipelines** — decomposing a problem into stages with a clear handoff (see GOLD-TRADING-SYSTEM: regime detection → signal generation → risk sizing → report), rather than one monolithic prompt.
- **Business-facing automation with an honest ROI model** — DOCUMENT-VERIFICATION-AGENT's business case is built from stated assumptions with the arithmetic shown, not a single confident number.
- **Applied ML end-to-end** — TrendHive (a university capstone, built with a 6-person team) combines Random Forest classifiers, SHAP explainability, an LSTM demand forecaster, and an agentic GPT-4o-mini/Claude copilot behind a FastAPI + React stack.

If you're evaluating whether an AI system you're building is actually doing what you think it's doing — or you need someone to build the extraction/validation/automation layer around an LLM rather than just the prompt — that's the work I want to be doing.

## Currently

- Open to freelance and full-time AI engineering roles
- Recent work: document verification agents, multi-agent trading/analysis pipelines, and a real-time computer vision surveillance stack (YOLOv8, ByteTrack, MediaPipe)

---

## Technology I've actually used (per my repos)

**Languages:** Python, TypeScript, JavaScript
**AI / LLM:** OpenAI API (gpt-4o-mini), Groq API (Qwen vision models), Pydantic-based structured output validation, SHAP, scikit-learn, TensorFlow/Keras (LSTM)
**Backend:** FastAPI, Supabase (PostgreSQL + Edge Functions), Next.js
**Interfaces:** Streamlit, React
**Computer vision:** YOLOv8 (Ultralytics), ByteTrack, MediaPipe, OpenCV
**Other:** PyMuPDF (PDF rasterization for vision models)

*(Not listed: anything I haven't shipped in a public repo. I'd rather this list be short and true than long and padded.)*

---

## Featured projects

### [Invoice Intake Agent](https://github.com/nathanmathew24/INTAKE-AGENT)
Upload an invoice, get back a validated, typed record. A vision-language model reads the document directly (no OCR step — layout is the signal that tells subtotal from total), Pydantic validates the extraction, and failed validations are fed back to the model as specific, actionable errors for up to three retries.
**[Live demo →](https://intake-agent-mujccynvv8jsxdgikvp8qf.streamlit.app/)**

### [Operations Copilot (Document Verification Agent)](https://github.com/nathanmathew24/DOCUMENT-VERIFICATION-AGENT)
A document/KYC case-review copilot — built with a teammate — with a full backend, frontend, and agent layer. Includes a from-first-principles business value model: every ROI number is traced back to a stated assumption, with three named scenarios (conservative/base/optimistic) rather than one number to defend.

### [Gold Trading System](https://github.com/nathanmathew24/GOLD-TRADING-SYSTEM)
A four-agent pipeline — regime detection, momentum signal generation, risk sizing, and an AI-narrated report — that produces a rules-based trade thesis for Gold futures from one command. Educational project; not investment advice.

### [TrendHive Market Intelligence](https://github.com/nathanmathew24/Project-Trend-Hive)
A university capstone project (team of 6): a full ML pipeline — Random Forest growth/popularity classifiers with SHAP explainability, an LSTM demand forecaster, and an agentic GPT-4o-mini/Claude copilot — behind a FastAPI backend and React dashboard, analyzing 500,000+ reviews across Dubai's café market.

### [Smart Surveillance System](https://github.com/nathanmathew24/SMART-SURVEILLANCE-CV)
A real-time computer vision app combining five techniques — MOG2 background subtraction, YOLOv8 object detection, YOLOv8+ByteTrack tracking, MediaPipe face detection, and YOLOv8 instance segmentation — behind a FastAPI backend and Streamlit frontend. University group project.

---

## Get in touch

- Email: [nxthxnmxthew7@gmail.com](mailto:nxthxnmxthew7@gmail.com)
- LinkedIn: [nathan-mathew-126273218](https://www.linkedin.com/in/nathan-mathew-126273218/)

---

*If a repo of mine is missing a README, it's a prototype I haven't finished documenting yet — not evidence it doesn't work. Open an issue if you want context on something specific.*
