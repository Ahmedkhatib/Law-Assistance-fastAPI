# Legal Chat Assistant 🧑‍⚖️

The **Legal Chat Assistant** is a FastAPI-based REST API that provides legal assistance on topics related to law, judiciary, justice, advocates, lawyers, and judgment-related matters. It uses the **Google Gemini Pro** model to generate accurate and professional responses to user queries.

---

## Features

- **Legal Expertise**: Specializes in Indian law, IPC sections, justice, advocates, lawyers, and judgment-related topics.
- **Session-Wise Conversations**: Saves conversation history for each session.
- **API Key Rotation**: Automatically switches to the next API key if the current one expires or reaches its limit.
- **REST API**: Provides a `/chat` endpoint for interacting with the assistant.

---

## How It Works

1. The user sends a `POST` request to the `/chat` endpoint with a `session_id` and `prompt`.
2. The app sends the prompt to the **Google Gemini Pro** model via its API.
3. The model generates a response based on the input and conversation history.
4. The response is returned to the user, and the conversation is saved for future reference.

---

## Setup Instructions

### Prerequisites

- Python 3.8 or higher
- A **Google Gemini API key** (get it from [Google AI Studio](https://makersuite.google.com/))

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/legal-chat-assistant.git
   cd legal-chat-assistant
