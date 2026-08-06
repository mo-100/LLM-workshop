# LLM Workshop

A hands-on workshop introducing Large Language Models (LLMs) and how to build with them.

## Prerequisites

- Basic understanding of Python programming concepts
- A laptop

## Topics Covered

1. **What Are LLMs?** — Transformer architecture, tokens, parameters, context length, popular models and use cases
2. **Basic LLM Usage** — Prompting, low-level (`transformers`) vs high-level (`openai` API) interfaces, running local models with [Ollama](https://ollama.com), generation hyperparameters (`temperature`, `top_p`, `top_k`, `max_tokens`), hallucination, tokenization
3. **Prompt Engineering** — Zero-shot, few-shot, chain-of-thought, role prompting, and structured output parsing with [Pydantic](https://docs.pydantic.dev/)
4. **Retrieval-Augmented Generation (RAG)** — Text embeddings, similarity metrics, vector databases with [FAISS](https://github.com/facebookresearch/faiss), chunking, and a full RAG pipeline
5. **Finetuning** — When and why to fine-tune, quantization with `bitsandbytes`, special tokens and chat templates
6. **Tool Calling** — Function calling, executing tools from LLM output, and security considerations
7. **Agents** — LLMs as reasoning engines with orchestrator-worker-reviewer workflows

## Getting Started

Clone the repository and install the dependencies:

```bash
git clone https://github.com/mo-100/LLM-workshop.git
cd LLM-workshop
pip install -r requirements.txt
```

### API Keys

The notebook uses [Google AI Studio](https://aistudio.google.com) to access Gemini models through the OpenAI-compatible API. Get a free API key there and store it as a Colab secret named `GEMINI_API_KEY`, or set it as an environment variable.

### Running Locally with Ollama

To run models on your own machine, install [Ollama](https://ollama.com) and pull a model:

```bash
ollama run qwen2.5:1.5b
```

## Requirements

See [requirements.txt](requirements.txt) for the full list of Python dependencies.

## License

This project is provided for educational purposes.
