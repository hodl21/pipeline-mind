# pipeline-mind 🧠

A multi-agent AI system that ingests your data, remembers what it saw, and tells you what changed in plain English.

Three Claude-powered agents collaborate: one profiles your data, one analyzes trends and compares against previous runs, one writes you a plain-English briefing. Built on raw Claude API + SQLite. No LangChain. No Docker. Runs locally.

---

## Quickstart

```bash
git clone https://github.com/hodl21/pipeline-mind.git
cd pipeline-mind
pip install -r requirements.txt
cp .env.example .env  # add your Anthropic API key
python run.py --source data/sample.csv
```

---

## Stack

| Layer | Tool |
|---|---|
| LLM | Claude (Anthropic API) |
| Memory | SQLite |
| Data profiling | pandas |
| UI | Streamlit |

---

## Roadmap

- [x] Architecture + README
- [ ] Memory layer (SQLite)
- [ ] Ingestion Agent
- [ ] Analysis Agent
- [ ] Report Agent
- [ ] Pipeline orchestrator
- [ ] Streamlit dashboard
