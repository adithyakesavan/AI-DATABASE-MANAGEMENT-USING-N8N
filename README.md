# AI-Powered Database Chat Agent (n8n Workflow)

An automated n8n workflow that connects a Large Language Model (OpenAI) to a PostgreSQL database using an AI Agent. This allows users to converse with their database using natural language rather than writing complex SQL queries.

## 🚀 Visual Workflow!
[n8n Workflow Canvas](./image.png)
*(Tip: Take a high-quality screenshot of your canvas and place it here)*

## 🛠️ Tech Stack & Nodes Used
* **n8n:** Workflow automation platform.
* **AI Agent Node:** To reason and decide when to fetch data.
* **OpenAI Chat Model:** Handles the natural language processing.
* **PostgreSQL:** The target database being queried.
* **Simple Memory:** Keeps track of the chat history for context.

## ⚙️ How It Works
1. **Trigger:** The workflow triggers when a chat message is received.
2. **Processing:** The AI Agent evaluates the user's prompt.
3. **Execution:** If data is needed, the Agent dynamically calls the Postgres node, executes the query, and formats the answer back to the user.

## 📦 How to Import This into Your n8n
1. Download the `chat-with-database-workflow.json` file from the `workflow/` folder in this repository.
2. Open your n8n instance.
3. Create a new workflow, click the top-right menu, and select **Import from File**.
4. Configure your own credentials for **OpenAI** and **PostgreSQL**.
