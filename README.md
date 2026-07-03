# 🤖 GEHU Chatbot - B.Tech CSE Department

> A rule-based chatbot for Graphic Era Hill University's B.Tech Computer Science and Engineering department — designed to assist students with ERP, results, fees, and department-related queries.

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Web-green?logo=flask&logoColor=white)
![HTML](https://img.shields.io/badge/HTML-5-orange?logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-3-blue?logo=css3&logoColor=white)

---

## 📌 Overview

This project is a **rule-based chatbot** specifically designed for the B.Tech Computer Science and Engineering department at Graphic Era Hill University. It helps students with common queries related to ERP login, result checking, fee submission, and department information through a clean web-based interface powered by Python Flask.

---

## 🎯 Objective

- Assist B.Tech CSE students with instant answers to common queries
- Provide quick access to ERP and department website links
- Reduce repetitive support workload for department staff
- Serve as a 24/7 automated assistant for student inquiries

---

## ✨ Key Features

- 💬 **Intelligent matching** — uses fuzzy string matching to find the best response
- 🧠 **JSON knowledge base** — easily extendable Q&A pairs stored in `knowledge_base.json`
- 🌐 **Modern web interface** — clean, responsive chat UI with gradient styling
- ⚡ **Python Flask backend** — lightweight server handles request/response logic
- 🔧 **Easy to customize** — add new responses by simply editing the JSON file
- 🔗 **Quick links** — direct access to ERP login and department website

---

## 🛠️ Tools & Technologies

| Technology | Role |
|---|---|
| Python (Flask) | Backend server & chatbot logic |
| HTML | Chat interface structure |
| CSS | Modern styling with gradients and responsive design |
| JSON | Knowledge base / response mapping |
| difflib | Fuzzy string matching for better query understanding |

---

## 📁 Project Structure

```
CHATBOT-main/
│
├── main.py                  # Flask app & chatbot logic
├── knowledge_base.json      # Predefined Q&A response data
├── README.md                # Project documentation
│
├── templates/
│   └── index.html           # Main chat interface (HTML)
│
└── static/
    ├── style.css            # Chatbot UI styling
    ├── GEHU-logo.png        # University logo
    ├── GEHU-Dehradun-1abd6f9c.jpg  # Campus image
    ├── Untitled.png         # Background image
    └── images.jpg           # Additional image
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- pip (Python package manager)

### Installation

```bash
# Clone the repository
git clone https://github.com/gurmej2004-gs/CHATBOT.git
cd CHATBOT-main

# Create a virtual environment
python3 -m venv venv

# Activate the virtual environment
# On macOS/Linux:
source venv/bin/activate
# On Windows:
# venv\Scripts\activate

# Install Flask
pip install flask
```

### Run the Chatbot

```bash
# Make sure the virtual environment is activated
python main.py
```

Then open your browser and navigate to:

```
http://127.0.0.1:5000
```

---

## 🧩 How It Works

1. User types a message in the web interface
2. The message is sent to the Python Flask backend
3. The backend uses fuzzy string matching to find the closest question in `knowledge_base.json`
4. The corresponding answer is returned and displayed in the chat UI
5. If no match is found (below 60% similarity), a fallback response is shown

---

## 📖 Extending the Knowledge Base

To add new responses, simply edit `knowledge_base.json`:

```json
{
    "questions": [
        {
            "question": "Your new question here",
            "answer": "Your custom answer here. You can include <a href='URL'>links</a>."
        }
    ]
}
```

The chatbot uses `difflib.get_close_matches()` with a 60% cutoff for fuzzy matching, so similar questions will still be recognized.

---

## � Important Links

- **ERP Portal:** https://student.gehu.ac.in
- **Department Website:** http://btechcsegehu.in/

---

## 💡 Supported Queries

The chatbot can help with:
- Greetings and general conversation
- ERP login assistance
- Result checking procedures
- Fee submission steps
- Department website information
- Contact department queries

---

## 🎓 Skills Demonstrated

- ✅ Python backend development (Flask)
- ✅ Frontend design with HTML & CSS
- ✅ JSON data structuring & parsing
- ✅ Fuzzy string matching for query understanding
- ✅ Full-stack web application development
- ✅ Git version control and GitHub integration

---

## 📝 Future Enhancements

- [ ] Add more comprehensive Q&A pairs
- [ ] Implement conversation history
- [ ] Add admin panel for easy knowledge base editing
- [ ] Integrate with actual ERP API for real-time data
- [ ] Add multilingual support

---

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Add new questions and answers to the knowledge base
- Improve the UI/UX design
- Fix bugs or enhance functionality
- Update documentation

---

## 📧 Contact

For questions or suggestions about this chatbot, please contact the B.Tech CSE department at Graphic Era Hill University.

---

