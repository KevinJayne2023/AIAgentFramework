# 🧠 A Simple Agent Framework with LiteLLM

This project demonstrates a minimal yet functional **AI Agent Loop** using the [LiteLLM](https://github.com/BerriAI/litellm) library, designed to simplify and streamline prompt/response handling with LLMs like OpenAI's GPT-4o.

---

## 🚀 Features

- 🧩 **Prompt Abstraction**: Easily create prompt objects containing messages, tools, and metadata.
- 🔁 **Agent Loop Logic**: An extendable loop system that feeds output back into the agent for multi-turn interactions.
- 🔐 **Secure API Key Handling**: Uses Colab’s `userdata` to keep your API key safe.
- ⚙️ **Tool Integration**: Supports tool-calling workflows, extensible via `functions` field.
- 💬 **Streamlined Response Handling**: Uses `litellm.completion` to fetch model outputs efficiently.

---

## 📦 Dependencies

Make sure you install the required package:

```bash
pip install litellm
```

## 📁 Usage

Open the notebook in **Google Colab**.

Click the 🔑 icon on the left to set your `OPENAI_API_KEY`.

Use the 📂 icon to upload any context files for the agent.

Run the cells to initialize the agent loop and start interacting.

---

## 🧰 Core Components

- **Prompt**: A dataclass that wraps `messages`, `tools`, and `metadata`.
- **generate_response(prompt)**: Calls the LLM and returns output.
- **Loop logic**: A basic flow that repeatedly calls the LLM and handles tool-use when needed.

---

## 🧪 Example Use Cases

- Autonomous tool-based question answering  
- Multi-turn task resolution  
- Educational reference for building LLM agents

---

## 📌 Notes

This framework is intentionally kept simple for learning and prototyping.

You can easily expand it by defining additional tools and handlers.
