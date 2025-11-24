# Agentic AI Using AutoGen, Gemini & Gradio

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![AutoGen](https://img.shields.io/badge/AutoGen-Latest-green.svg)](https://github.com/microsoft/autogen)
[![Gemini](https://img.shields.io/badge/Google-Gemini%202.5-orange.svg)](https://ai.google.dev/)
[![Gradio](https://img.shields.io/badge/Gradio-UI-ff6f61.svg)](https://gradio.app/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

This project demonstrates how to build agentic AI systems using Microsoft AutoGen, Google Gemini models, and a Gradio-based interactive interface. It shows how multiple intelligent agents can collaborate, communicate, and solve tasks autonomously, powered by large-language-model reasoning.

---

## Overview

**What This Project Does:**

- Uses AutoGen to create and manage multiple cooperative AI agents
- Integrates Google Gemini (2.5-Flash) through ag2 for fast and cost-efficient reasoning
- Builds an interactive Gradio UI where users can submit queries and watch agents collaborate
- Loads API keys securely using python-dotenv
- Demonstrates agent-to-agent conversations, problem solving, and dynamic task execution

In short: A complete agentic AI demo that shows how LLM-powered agents can plan, reason, and respond automatically.

---

## Core Technologies

| Library | Purpose |
|---------|---------|
| **AutoGen (pyautogen)** | Multi-agent orchestration |
| **ag2 (Gemini integration)** | Google Gemini API wrapper |
| **Gradio** | UI for interacting with the agent system |
| **python-dotenv** | Secure environment variable loading |
| **Google Generative AI** | LLM backend (Gemini 2.5 Flash) |

---

## Project Structure

```
agentic-ai-autogen/
│
├── notebook.ipynb              # Main Jupyter notebook
├── .env                        # Environment variables (not committed)
├── .gitignore                  # Git ignore file
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation
```

The `.ipynb` file contains:
- Installation of dependencies
- Environment variable setup
- Gemini configuration (`config_list_gemini`)
- Agent definitions
- Gradio interface generation
- Agent conversation logic

---

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/agentic-ai-autogen.git
cd agentic-ai-autogen
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install pyautogen python-dotenv gradio google-generativeai "ag2[gemini]"
```

### 3. Configure Environment Variables

Create a `.env` file in the project root:

```env
GOOGLE_API_KEY=your_google_api_key_here
```

**Note:** Get your API key from [Google AI Studio](https://makersuite.google.com/app/apikey)

### 4. Run the Notebook

```bash
jupyter notebook notebook.ipynb
```

Open the notebook and run all cells.

---

## How to Use

1. Launch the notebook
2. A Gradio interface appears
3. Type any question or task
4. AutoGen agents + Gemini collaborate to generate the result

### Example Queries

- "Explain how reinforcement learning works."
- "Write a small Python script for data cleaning."
- "Plan a 3-day travel itinerary."

---

## How It Works

### 1. Gemini Model Configuration
The notebook loads your API key and prepares a unified Gemini config for all agents.

### 2. Agent Creation
AutoGen agents are defined (e.g., an Assistant agent and a UserProxy agent).

### 3. LLM-Based Collaboration
Agents communicate with each other using Gemini responses to solve tasks.

### 4. Gradio UI
A clean web interface lets you ask questions and view agent responses.

---

## Requirements

```txt
pyautogen>=0.2.0
python-dotenv>=1.0.0
gradio>=4.0.0
google-generativeai>=0.3.0
ag2[gemini]>=0.1.0
```

---

## Future Enhancements

- [ ] Add memory-enabled agents
- [ ] Add tool-use enabled agents (code execution, web search, etc.)
- [ ] Add conversation logs
- [ ] Add more agent roles (planner, critic, coder)
- [ ] Export conversations to JSON/CSV
- [ ] Deploy as a web application
- [ ] Add authentication and user sessions
- [ ] Integrate vector databases for RAG capabilities

---

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- [Microsoft AutoGen](https://github.com/microsoft/autogen) for the multi-agent framework
- [Google Gemini](https://ai.google.dev/) for the language model
- [Gradio](https://gradio.app/) for the UI framework

---

## Contact

For questions or feedback, please open an issue on GitHub.

---

**Built with AutoGen, Gemini, and Gradio**
