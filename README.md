# Rag API - ollama local models

### Install ollama

Windows - ollama.com (download .exe file)
Linux - curl -fsSL https://ollama.com/install.sh | sh

```bash
ollama pull gemma3:1b
curl http://localhost:11434
```

### Project setup

Requirement - python ^3.13

```bash
python3.13 --version

python3.13 -m venv venv
source venv/bin/activate
```

Install dependencies

```bash
pip install fastapi uvicorn chromadb ollama
ollama pull nomic-embed-text

ollama list
```

### Start API server

```bash
uvicorn main:app --reload
```

Open browser - http://127.0.0.1:8000/docs

Try it out -> Ask question