# 📄 AI Resume Builder

An **AI-powered Resume Builder** developed with **Streamlit** that helps users create professional resumes quickly and efficiently. The application allows users to enter their personal information, education, work experience, skills, and projects, while leveraging **Google Gemini AI** to generate or improve the **About Me** section in different writing styles.

The generated resume can be previewed, exported as a high-quality PDF, and automatically stored in a local **SQLite** database for future reference.

---

## ✨ Features

### 👤 Personal Information

* Add personal details including name, email, phone number, address, and professional links.
* Easy-to-use and responsive input forms.

### 🎓 Education

* Add multiple educational qualifications.
* Include institution name, degree, duration, and description.

### 💼 Work Experience

* Add unlimited work experience entries.
* Include company name, job title, duration, and responsibilities.

### 🚀 Projects

* Showcase academic or professional projects.
* Add project title, technologies used, and project description.

### 🛠 Skills

* Add technical and soft skills.
* Display skills in a clean and organized format.

### 🤖 AI-Powered About Me

Generate or improve your professional summary using **Google Gemini AI**.

Available writing styles:

* Professional
* Creative
* Catchy
* Detailed

### 🎨 Multiple Resume Templates

Choose from different professionally designed resume templates before generating your resume.

### 📄 PDF Export

Generate a polished PDF resume with one click using:

* Jinja2
* WeasyPrint

### 💾 SQLite Database

Every generated resume is automatically saved locally in a SQLite database.

### 🌙 Light & Dark Mode

Switch between Light and Dark themes for a better user experience.

---

# 🛠 Tech Stack

| Component             | Technology        |
| --------------------- | ----------------- |
| Frontend              | Streamlit         |
| AI Integration        | Google Gemini API |
| AI Library            | google-genai      |
| HTML Templates        | Jinja2            |
| PDF Generation        | WeasyPrint        |
| Database              | SQLite            |
| Environment Variables | python-dotenv     |

---

# 🚀 Getting Started

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/AI-Resume-Builder.git

cd AI-Resume-Builder
```

---

## 2. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 3. Configure Environment Variables

Create a `.env` file in the project root and add your Google Gemini API credentials.

Example:

```env
GEMINI_API_KEY=your_actual_api_key_here

GEMINI_MODEL=gemini-flash-latest
```

You can obtain a free API key from **Google AI Studio**.

---

## 4. Run the Application

```bash
streamlit run app.py
```

After running the command, open your browser and visit:

```
http://localhost:8501
```

---

# 📁 Project Structure

```text
AI-Resume-Builder/
│
├── app.py                 # Main Streamlit application
├── database.py            # SQLite database operations
├── templates.py           # Resume HTML templates
├── requirements.txt       # Project dependencies
├── .env.example           # Environment variable template
├── .gitignore
├── README.md
└── resume_data.db         # Auto-generated SQLite database
```

---

# 🗄️ Database

The application automatically creates a SQLite database named:

```
resume_data.db
```

The database stores the following information:

### resumes

* Personal Information
* Contact Details
* About Me
* Skills

### education

* Degree
* Institution
* Duration
* Description

### experience

* Company
* Job Title
* Duration
* Responsibilities

### projects

* Project Title
* Technologies Used
* Description

Each section is linked through a unique **resume_id**.

You can inspect the database using:

* SQLite Viewer (VS Code Extension)
* SQLTools Extension
* DB Browser for SQLite

---

# 📦 Python Libraries Used

* streamlit
* google-genai
* python-dotenv
* Jinja2
* WeasyPrint
* sqlite3

---

# 📌 Future Improvements

* User Authentication
* Cloud Database Integration
* Resume Sharing via Link
* Download in DOCX Format
* More Resume Templates
* Profile Photo Upload
* ATS Resume Score
* Resume Editing History

---

# 🤝 Contributing

Contributions are welcome.

If you'd like to improve this project:

1. Fork the repository.
2. Create a new feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

---

# 📄 License

This project is developed for educational and learning purposes.

Feel free to use and modify it for personal or academic projects.

---

# 👩‍💻 Author

**Tatheer Fatima**

Software Engineering Student

AI | Python | Streamlit | Web Development

⭐ If you found this project useful, don't forget to **Star** the repository.
