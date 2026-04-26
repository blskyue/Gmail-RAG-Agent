Gmail-RAG-Agent 📧🤖
A Retrieval-Augmented Generation (RAG) agent that interacts with your Gmail account. It allows you to search through your emails using semantic understanding and perform actions like sending new messages directly through the AI.

🚀 Overview
Unlike traditional keyword-based email search, this agent utilizes Semantic Search to find relevant information. It processes your inbox through a specialized pipeline: Load, Embed, Store, and Retrieve.

🛠️ Tech Stack
Frameworks: LangChain & LangGraph

LLM: Anthropic's Claude Opus 3.5 (via OpenRouter)

Embeddings: HuggingFace (all-mpnet-base-v2)

Vector Store: InMemoryVectorStore

API Integration: Gmail API & IMAP

✨ Features
Contextual Understanding: Uses advanced embeddings to capture the intent behind your email queries.

Smart Retrieval: Searches your private email datasets to answer specific questions like "Did I receive any invitations?".

Autonomous Actions: Capability to compose and send emails using the Gmail API based on natural language instructions.

Memory & State: Maintains conversation history using InMemorySaver, allowing for smooth follow-up questions.

⚙️ Setup & Authentication
IMAP: Used for fetching emails. Ensure you use an App Password for your Gmail account.

Gmail API: Create a project in Google Cloud Console, enable Gmail API, and download credentials.json.

Secrets: Store GMAIL_USERNAME, GMAIL_PASSWORD, and OPENROUTER_API_KEY in your environment or Colab Secrets.
