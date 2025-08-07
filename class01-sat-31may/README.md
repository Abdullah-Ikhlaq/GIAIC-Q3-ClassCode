# Multi-Agent Gemini Client using OpenAI Agent SDK

This is a Python project that demonstrates how to create and run **multiple AI agents** (e.g., a Math teacher and English teacher) using the **OpenAI Agent SDK**, powered by **Gemini 2.0** via Google's API.


## Features

- Integrates with **Gemini 2.0 Flash** through the OpenAI Agent SDK
- Defines multiple conversational agents (Math & English teachers)
- Agent execution via `Runner.run_sync()`
- Environment-based API key loading via `python-decouple`


## Tech Stack

|        Tool        |              Purpose               |
|--------------------|------------------------------------|
|      `openai`      | Async client setup for Gemini API  | 
|   `openai.agent`   | To create AI agents and runners    |
| `python-decouple`  | Secure API key handling via `.env` |
| `Gemini 2.0 Flash` | Language model used in agents      |


## Requirements

Make sure to install the required dependencies:

```bash
pip install openai python-decouple
```

## Environment Setup

Create a .env file in the root directory and add your Gemini API key:

```bash
GEMINI_API_KEY=your_gemini_api_key_here
```

## File Structure
```bash
├── .env.example
├── main.py
├── pyproject.toml
├── .python-version
├── uv.lock 
└── README.md
```

## Example Output
```bash
> what is 2 + 2?
Answer: 4
```

## Notes
- `english_agent` is defined but not used. You can extend the app to take dynamic input or run multiple agents in parallel.

- Be sure to handle API usage according to rate limits and pricing for Gemini API.


## License

This project is licensed under the MIT License.


## Author
Made with ❤️ by Abdullah Ikhlaq