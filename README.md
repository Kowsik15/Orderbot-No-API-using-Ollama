# 🍕 OrderBot - Chatbot Without API Using Ollama + LangChain

A conversational chatbot that takes pizza orders using a local Large Language Model (LLM) powered by [Ollama](https://ollama.com/) and [LangChain](https://www.langchain.com/). This project runs **entirely offline** without needing OpenAI or external APIs.

---

## 🧠 Features

* Fully offline, no internet or API key required
* Built with **LangChain + Ollama** (local Mistral model)
* User-friendly pizza ordering chatbot UI using **Gradio** or **Panel**
* Supports:

  * Menu interpretation
  * Order collection (size, quantity, toppings)
  * Pickup or delivery options
  * Payment confirmation
* Easy customization of prompts and menu

---

## 🏋️ Sample Menu Prompt

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

### 1. Install Ollama and Pull the Mistral Model

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

### 3. Run the Chatbot

Choose either of the following UI options:

#### Option A: Gradio Chat UI

* Create a Python script or Jupyter notebook and launch using `demo.launch()`

#### Option B: Panel-based Chat Interface

* Use Panel’s `dashboard.show()` to serve a local app

---

## 📆 Project Structure

* `Chatbot_NoAPI_Ollama.ipynb`: Main notebook for chatbot logic
* `README.md`: Project documentation
* `requirements.txt`: Python dependency list

---

## 🧹 Tech Stack

| Tool          | Purpose                           |
| ------------- | --------------------------------- |
| **LangChain** | Message formatting and flow       |
| **Ollama**    | Local LLM serving (Mistral model) |
| **Gradio**    | Web-based UI interface            |
| **Panel**     | Alternative desktop-like UI       |

---

## ✅ TODOs

* [x] Local chatbot setup using LangChain + Ollama
* [x] Integrate both Gradio and Panel UIs
* [ ] Implement order summary display
* [ ] Enable session-based order history
* [ ] Add voice interface (optional)

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

**MIT License** – Free to use, distribute, and modify.

```
MIT License

Copyright (c) 2025 Kowsik.S

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the “Software”), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
of the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

---

## 🙌 Acknowledgements

* [Ollama](https://ollama.com/) for enabling offline LLMs
* [LangChain](https://www.langchain.com/) for language model workflows
* [Gradio](https://www.gradio.app/) & [Panel](https://panel.holoviz.org/) for easy UI integration
