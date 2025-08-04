
# 🍕 OrderBot - Chatbot Without API Using Ollama + LangChain

A conversational chatbot that takes pizza orders using a local Large Language Model (LLM) powered by [Ollama](https://ollama.com/) and [LangChain](https://www.langchain.com/). This project runs **entirely offline** without needing OpenAI or external APIs.

---

## 🧠 Features

- Built with **LangChain + Ollama** (local Mistral model)
- Interactive pizza ordering chatbot UI using **Gradio** or **Panel**
- Handles:
  - Menu interpretation
  - Order collection
  - Pickup/delivery instructions
  - Payment confirmation
- Fully customizable prompts & menu
- No internet or API key required

---

## 📋 Menu (Sample Prompt)

```
pepperoni pizza  12.95, 10.00, 7.00  
cheese pizza     10.95, 9.25, 6.50  
eggplant pizza   11.95, 9.75, 6.75  
fries            4.50, 3.50  
greek salad      7.25  

Toppings:  
extra cheese 2.00  
mushrooms 1.50  
sausage 3.00  
canadian bacon 3.50  
AI sauce 1.50  
peppers 1.00  

Drinks:  
coke 3.00, 2.00, 1.00  
sprite 3.00, 2.00, 1.00  
bottled water 5.00  
```

---

## 🛠️ Installation & Setup

### 1. Install Ollama and Pull Mistral Model
```bash
# Download Ollama
https://ollama.com/download

# After installation:
ollama run mistral
```

### 2. Set Up Python Environment

Install dependencies:
```bash
pip install langchain ollama gradio panel
```

### 3. Run the Bot

Use either interface:

#### Option A: Gradio Chat UI
```python
# run this block in a .py file or notebook
import gradio as gr
from langchain.chat_models import ChatOllama
...

demo.launch()
```

#### Option B: Panel-based Chat Interface
```python
import panel as pn
pn.extension()

# run the dashboard
dashboard.show()
```

---

## 📦 Files

- `Chatbot_NoAPI_Ollama.ipynb`: Main notebook with full working chatbot
- `README.md`: Project documentation
- `requirements.txt`: Dependencies

---

## 🧩 Tech Stack

| Tool        | Purpose                      |
|-------------|------------------------------|
| LangChain   | Chat message formatting & flow |
| Ollama      | Local LLM serving (Mistral)  |
| Gradio / Panel | UI for user interaction    |

---

## ✅ TODOs

- [x] Setup local chatbot
- [x] Integrate Panel and Gradio
- [ ] Add order summary breakdown
- [ ] Store past orders (session-based)
- [ ] Optional: Add voice interface

---

## 💬 Example Conversation

```
User: Hi  
Bot: Hey there! Welcome to our pizza place. What can I get started for you today?

User: I want a large pepperoni pizza and a small coke.  
Bot: Got it! One large pepperoni pizza 🍕 and a small coke 🥤. Will that be for pickup or delivery?
```

---

## 📄 License

MIT License – feel free to use and modify.

---

## 🙌 Acknowledgements

- [Ollama](https://ollama.com/) for offline LLM serving
- [LangChain](https://www.langchain.com/) for seamless LLM integrations
- Gradio & Panel for rapid UI prototyping
