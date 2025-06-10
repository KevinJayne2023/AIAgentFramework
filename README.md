# Simple Litellm-Powered Agent Framework

A lightweight, extendable agent loop built on Google Colab using [litellm](https://pypi.org/project/litellm). This framework lets you define goals, register custom actions (tools), maintain memory, and have your agent autonomously decide and execute steps until termination.

---

## 🔧 Features

- **Goal-Driven Loop**  
  Define one or more `Goal`s with priorities; the agent keeps working until a terminal goal is reached.

- **Pluggable Actions**  
  Register any Python function as an `Action` with a name, description, JSON schema for parameters, and a `terminal` flag.

- **Function-Calling with LLM**  
  Uses GPT-4o function-call support to choose and invoke your actions, passing arguments via `**args`.

- **Simple Memory Store**  
  Maintains working memory of user inputs, agent decisions, and environment results; filters or copies memory as needed.

- **Environment Abstraction**  
  Wraps action execution to catch errors, attach timestamps, and format results uniformly.

---

## 🚀 Getting Started

1. **Clone & Open in Colab**  
   ```bash
   git clone https://github.com/your-org/your-repo.git
