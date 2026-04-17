# OrderBot 🍕

## Overview
OrderBot is a conversational AI prototype built as part of the **ChatGPT Prompt Engineering for Developers** course by DeepLearning.AI.  
It demonstrates how a chatbot can be designed around **system instructions, conversation history, and a response loop** to deliver domain‑specific interactions.

## How It Works
- **System Message**: Defines the bot’s role, rules, and domain knowledge (FoodHut menu and ordering flow).  
- **Conversation History**: Maintains context across turns by appending user and assistant messages.  
- **Response Generation Loop**: Sends the full history to a chat‑trained model via Hugging Face Inference API, receives a reply, and updates the history.  
- **Reset Function**: Clears the conversation and restores only the system message, effectively restarting the bot while preserving its identity.  
- **UI Layer**: Built with `ipywidgets` in Jupyter Notebook, featuring a chat display, input box, send button, and reset button.

## Features
- Warm, friendly ordering flow with contextual awareness.  
- Menu‑driven responses that block unrelated queries (e.g., news requests).  
- Stateful conversation management.  
- Reset button for restarting sessions.  

## Tech Stack
- **Python**  
- **Hugging Face Hub** (`InferenceClient`)  
- **Jupyter Notebook + ipywidgets** for UI  

## Learning Outcomes
This project illustrates the **core principles of prompt engineering**:
- Defining assistant behavior through a hidden system instruction block.  
- Maintaining dialogue state for contextual consistency.  
- Enforcing domain boundaries via system prompts (context blocking).  
- Building a minimal but functional UI for interactive demos.  

## Next Steps
- Migrate UI to **Gradio/Streamlit/Dash** for browser‑based deployment.  
- Dockerize the app for portable demos.  
- Extend prompt engineering modules (Basics, Expanding, Inferring, Summarizing, Transforming) into structured interview prep notes.
