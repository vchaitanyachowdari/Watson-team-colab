# 🚀 Mindmap Generator AI

**Mindmap Generator AI** is an open-source tool that transforms plain text documents into structured, visual mindmaps using AI — ideal for brainstorming, note-taking, and learning.

---

## 📘 Table of Contents

* [Features](#features)
* [Demo](#demo)
* [Installation](#installation)
* [Usage](#usage)
* [Configuration](#configuration)
* [Architecture](#architecture)
* [Development](#development)
* [Contributing](#contributing)
* [License](#license)
* [Contact](#contact)

---

## ⚙️ Features

* AI-powered parsing of text into hierarchical concepts
* Export mindmaps as JSON / Markdown / visual image
* CLI interface + optional web frontend
* Customizable via config file or command-line flags

---

## 🎥 Demo

🔗 *Insert link to demo GIF, image, or hosted app*

---

## 🛠️ Installation

### Prerequisites

* Python 3.8+
* Node.js (if frontend/UI included)
* (Optional) Virtualenv or Conda

### Setup

```bash
git clone https://github.com/vchaitanyachowdari/mindmap-generator-ai.git
cd mindmap-generator-ai

# (Optional) create a virtual environment
python -m venv .venv && source .venv/bin/activate

pip install -r requirements.txt
```

---

## 🚀 Usage

### CLI

```bash
python generate_mindmap.py \
  --input path/to/input.txt \
  --output mindmap.json \
  --format json \
  --model gpt-3.5-turbo \
  # other flags...
```

### Programmatic

```python
from mindmap import generate

mindmap = generate(
    text="Your input text here...",
    model="gpt-3.5-turbo",
    max_depth=4
)
print(mindmap)
```

### Web UI (If available)

```bash
cd ui
npm install
npm run dev
# then open http://localhost:3000
```

---

## ⚙️ Configuration

| Setting          | Description            | Default           |
| ---------------- | ---------------------- | ----------------- |
| `model`          | OpenAI model to use    | `gpt-3.5-turbo`   |
| `max_depth`      | Maximum mindmap depth  | `3`               |
| `output_format`  | `json`, `md`, or `png` | `json`            |
| `openai_api_key` | Your OpenAI API key    | *None (required)* |

You can pass these via flags, config file, or environment variables.

---

## 🧱 Architecture

1. **Text Processor** – splits and categorizes input text.
2. **AI Module** – prompts OpenAI to extract nodes and hierarchy.
3. **Formatter** – converts raw output to JSON, Markdown, and optionally HTML/SVG.
4. **CLI / UI** – user entrypoints.

---

## 💻 Development

### Setup

```bash
# Already installed dependencies above
```

### Run tests

```bash
pytest
```

### Linting

```bash
flake8 .
black .
```

---

## 🤝 Contributing

We welcome contributions! Please:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/foo`)
3. Commit your changes (`git commit -am 'Add foo'`)
4. Push to your branch (`git push origin feature/foo`)
5. Open a pull request

✅ Please follow the [Contributor Code of Conduct](CODE_OF_CONDUCT.md).

---

## 📄 License

This project is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.

---

## 📞 Contact

Created by **vchaitanyachowdari**
Feel free to reach out at: [GitHub Issues](https://github.com/vchaitanyachowdari/mindmap-generator-ai/issues)

Enjoy building mindmaps! 🎉
