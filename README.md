# Rag API + Ollama Local models

## Install ollama

`Windows` - [Ollama](ollama.com) (download .exe file)

```bash
#Linux
curl -fsSL https://ollama.com/install.sh | sh

ollama pull gemma3:1b
curl http://localhost:11434
```

## Project setup

Requirement - python ^3.13

```bash
# check python
python3.13 --version

<<<<<<< HEAD
# Create a virtual environment
=======
# create venv
>>>>>>> 0c93273 (Update setup with requirements.txt)
python3.13 -m venv venv
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt

# ollama setup
ollama pull nomic-embed-text
ollama list
```

## Start API server

```bash
uvicorn main:app --reload
```

Open browser - http://127.0.0.1:8000/docs

## Testing

Click `Try it out` -> Ask question
