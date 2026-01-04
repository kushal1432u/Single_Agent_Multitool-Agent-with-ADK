# Agent Development Kit (ADK) 🛠️🤖

**ADK** is a powerful development and debugging environment for building complex AI agents. It provides a real-time "observability" layer, allowing developers to trace agent reasoning, monitor state changes, and evaluate multi-step task execution in a unified dashboard.

---

## 🚀 Key Features

* **Real-Time Trace & Observability:** Monitor the "chain-of-thought" as the agent processes complex requests (e.g., travel planning or logistical routing).
* **State Management:** Inspect the agent's internal memory and state transitions at every step of the process.
* **Invocation Tracking:** View a history of all tool calls and logic branches triggered during a session.
* **Session Management:** Maintain multiple isolated chat sessions with unique IDs for testing and comparison.
* **Artifact & Event Logging:** Deep-dive into specific data artifacts produced by the agent or events triggered by the system.
* **Token Streaming:** Toggle real-time output streaming for a smoother user experience.

---

## 🛠️ Technical Stack

* **Frontend:** React-based Web UI (ADK Web Developer UI)
* **Agent Logic:** Python (utilizing LangGraph or LangChain for stateful workflows)
* **Observability:** OpenTelemetry-compatible tracing or custom event streaming
* **API:** WebSocket/REST for real-time agent interaction

---

## 📸 Dashboard Overview

1.  **Sidebar (Control Center):** Select your agent, view traces, events, state, and evaluation metrics.
2.  **Invocations Panel:** A detailed list of every action the agent has taken.
3.  **Chat Canvas:** A clean interface to interact with the agent, supporting attachments, voice input, and video.
4.  **Metadata Bar:** Displays Session ID, User ID, and token usage toggles.

---

## 💻 Installation

1. **Clone the repository**
   ```bash
   git clone [https://github.com/yourusername/agent-development-kit.git](https://github.com/yourusername/agent-development-kit.git)
   cd agent-development-kitSetup Backend

Bash

pip install -r requirements.txt
python main.py
Setup Frontend

Bash

cd ui
npm install
npm start
💡 Example Use Case: Travel Planning Agent
As seen in the demo, the ADK helps debug agents that require multi-modal logistics:

Step 1: Identifying local transport (Gadag to Hubballi).

Step 2: Sourcing domestic flight connections (Hubballi to Bengaluru/Mumbai).

Step 3: Managing international airline requirements (Visa, Passport, Luggage).

📝 License
Distributed under the MIT License.
