Here's a beautiful and complete `README.md` for your **Course Recommendation Bot** project, designed to impress recruiters, teachers, and GitHub visitors. It includes all major sections with badges, features, setup, demo, and credits.

---

```markdown
# 🎓 Course Recommendation Bot using IBM Watsonx.ai

![Python](https://img.shields.io/badge/Python-3.10-blue.svg)
![Django](https://img.shields.io/badge/Django-4.x-green.svg)
![Watsonx](https://img.shields.io/badge/IBM-watsonx.ai-ff9900?logo=ibm)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

An AI-powered course recommendation system that uses IBM Watsonx.ai's Foundation Models and Django to provide smart, tailored course suggestions based on user interests. Built with a clean UI, dynamic prompt engineering, and CSV-driven knowledge base.

---

## 📸 Demo

![Course Recommender UI Demo](https://user-images.githubusercontent.com/yourusername/demo-image.gif)

> _"Just type what you're interested in, and our AI finds the best learning paths for you!"_

---

## 🚀 Features

- 🧠 **Watsonx.ai Integration** for natural language understanding and generation
- 📚 **CSV-based Course Dataset** with 250+ curated course entries
- 💡 **Interest-based Filtering** via keyword tagging (e.g., tech, business, mechanical, finance)
- ✨ **Beautiful UI** using Bootstrap 5 + CSS Glassmorphism
- 📤 **Smart Prompt Engineering** to guide foundation models to generate 5 precise recommendations
- 🔒 **Secure API Key Handling** using `.env` and Django settings

---

## 🏗️ Tech Stack

| Layer         | Technology                     |
|--------------|--------------------------------|
| 💬 Prompting  | IBM Watsonx.ai - Granite 3-8B Instruct |
| 🌐 Frontend   | HTML5, CSS3, Bootstrap 5       |
| ⚙️ Backend    | Django (Python)                |
| 📦 Data       | CSV (course_data_300.csv)      |
| 🔐 Auth       | IAM Token from IBM API Key     |

---

## 📁 Project Structure

```

Course-Recommendation-Bot/
│
├── static/                   # Styles and icons
├── templates/
│   └── index.html            # UI with input and response area
├── views.py                 # Django view logic
├── prompt\_api.py           # IBM watsonx.ai call and config
├── course\_data\_300.csv      # Knowledge base
├── settings.py              # API key and Django setup
├── .env                     # Stores WATSONX\_API\_KEY securely
└── README.md

````

---

## 🧪 How It Works

1. **User Input**: "I want to master machine learning."
2. **Keyword Matching**: Tags like `tech`, `AI`, `data` are matched.
3. **Course Fetch**: Matching entries are filtered from the CSV.
4. **Prompt Formulation**: A structured prompt is sent to Watsonx.ai.
5. **AI Response**: Returns 5 clean, formatted recommendations.
6. **Output Displayed**: Beautiful UI shows the results dynamically.

---

## ⚙️ Local Setup

```bash
git clone https://github.com/yourusername/course-recommendation-bot.git
cd course-recommendation-bot

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
touch .env
echo "WATSONX_API_KEY=your_ibm_api_key" >> .env

# Run the server
python manage.py runserver
````

Visit: [http://127.0.0.1:8000](http://127.0.0.1:8000)

---

## 📊 Sample Prompt Sent to Watsonx

```
You are a helpful course recommendation assistant. Based on the user's interests and the following available courses, suggest the top 5 most relevant courses...
```

✅ Output Format:

```
1. 🧠 Course Title (ID)
   One-line description.
...
```

---

## 📦 Dependencies

* Django
* Requests
* Python-dotenv
* IBM Watsonx Foundation Model API

---

## 🧠 Improvements

* [ ] Integrate real-time vector-based RAG
* [ ] User feedback & ratings
* [ ] Dynamic CSV uploads by admin
* [ ] Multi-language support

---

## 🙏 Credits

Made with ❤️ by **Garv Bhardwaj**
Powered by **IBM Watsonx.ai**
Designed for GENAI Final Submission 📘

> “Learning made smart. With AI.”
