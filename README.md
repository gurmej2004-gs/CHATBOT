# 🤖 Rule-Based Chatbot System

> A conversational chatbot built with Python, HTML, CSS & JSON — designed to automate repetitive user queries with structured rule-based logic.



## 📌 Overview

This project is a **rule-based chatbot** designed to handle basic user queries through predefined responses. It demonstrates the use of structured logic for automated interaction and query handling, with a clean web-based chat interface powered by a Python (Flask) backend.

---

## 🎯 Objective

- Automate repetitive and common user queries
- Improve response time with instant, predefined answers
- Reduce manual support workload through intelligent routing
- Serve as a foundation for more advanced AI chatbot systems

---

## ✨ Key Features

- 💬 **Rule-based response engine** — matches user input to predefined intents
- 🧠 **JSON knowledge base** — easily extendable Q&A pairs stored in `knowledge_base.json`
- 🌐 **Web interface** — clean, responsive chat UI built with HTML & CSS
- ⚡ **Python Flask backend** — lightweight server handles request/response logic
- 🔧 **Easy to customize** — add new responses by simply editing the JSON file

---

## 🛠️ Tools & Technologies

| Technology | Role |
|---|---|
| Python (Flask) | Backend server & chatbot logic |
| HTML | Chat interface structure |
| CSS | Styling and responsive layout |
| JSON | Knowledge base / response mapping |

---

## 📁 Project Structure

```
CHATBOT/
│
├── main.py                  # Flask app & chatbot logic
├── knowledge_base.json      # Predefined Q&A response data
│
├── templates/
│   └── index.html           # Main chat interface (HTML)
│
├── static/
│   ├── style.css            # Chatbot UI styling
│   └── script.js            # Frontend interaction logic
│
└── README.md                # Project documentation
```




## 🧩 How It Works

1. User types a message in the web interface
2. The message is sent to the Python Flask backend
3. The backend searches `knowledge_base.json` for a matching intent/keyword
4. A predefined response is returned and displayed in the chat UI
5. If no match is found, a fallback response is shown

---

## 📖 Extending the Knowledge Base

To add new responses, simply edit `knowledge_base.json`:

```json
{
  "intents": [
    {
      "tag": "greeting",
      "patterns": ["Hello", "Hi", "Hey"],
      "responses": ["Hello! How can I help you?", "Hi there! What can I do for you?"]
    },
    {
      "tag": "your_new_topic",
      "patterns": ["your keyword", "another keyword"],
      "responses": ["Your custom response here."]
    }
  ]
}
```

---

## 💡 Use Cases

- 🛎️ **Customer support automation** — answer FAQs instantly
- 🖥️ **Helpdesk systems** — route common IT or HR queries
- 🎓 **Educational tools** — quiz or tutoring bots
- 🤖 **Entry-level AI applications** — a great base to extend with ML/NLP

---

## 🎓 Skills Demonstrated

- ✅ Python backend development (Flask)
- ✅ Frontend design with HTML & CSS
- ✅ JSON data structuring & parsing
- ✅ Chatbot logic & intent-matching design
- ✅ Full-stack mini web application development

---

