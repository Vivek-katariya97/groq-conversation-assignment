# Conversation Management & Classification with Groq API

This project implements two core tasks using the Groq API: robust conversation history management and structured information extraction from user chats. The entire implementation is done in a Google Colab notebook using standard Python and the OpenAI SDK, without any external frameworks like LangChain.

---

## 🚀 Objective

The goal is to demonstrate the ability to manage conversational data, perform periodic summarization to keep context concise, and classify user chats to extract structured data into a predefined JSON schema.

---

## ✨ Features

### Task 1: Conversation Management & Summarization
- **Maintain History**: Keeps a running history of user-assistant interactions.
- **Periodic Summarization**: Automatically summarizes the conversation history after every `k`-th user turn to keep the context window small and relevant. The summary replaces the older part of the conversation.
- **Truncation by Turn Count**: Option to limit the conversation history to the last `n` turns.
- **Truncation by Length**: Option to limit the conversation history by a maximum character count, keeping only the most recent messages.

### Task 2: JSON Schema Classification & Information Extraction
- **Structured Extraction**: Uses Groq's tool-calling (function calling) feature to extract specific details from user chats.
- **Custom JSON Schema**: Defines a schema to extract 5 key details: `name`, `email`, `phone`, `location`, and `age`.
- **Validation**: The process inherently validates the extracted data against the defined JSON schema.

---

## 🛠️ Technologies Used

- **Language**: Python
- **API**: Groq API
- **SDK**: OpenAI Python SDK
- **Environment**: Google Colab

---

## ⚙️ Setup and Usage

1.  **Get a Groq API Key**:
    - Sign up or log in to the [Groq Console](https://console.groq.com/keys).
    - Create a new API key and copy it.

2.  **Open in Colab**:
    - Open the `.ipynb` file in Google Colab.

3.  **Run the Setup Cell**:
    - Run the first code cell. It will install the necessary libraries (`groq`, `openai`).
    - When prompted, paste your Groq API key.

4.  **Execute All Cells**:
    - Run the remaining cells in order by selecting **Runtime > Run all**.
    - The notebook will demonstrate each feature with clear outputs.

---

## 📂 Project Structure

```
.
└── your_notebook_name.ipynb      # Main Colab notebook with all code and demonstrations.
```
