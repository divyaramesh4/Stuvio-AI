## 📌 Project Overview

**Stuvio AI** is a web application designed to enhance learning by generating short, informative videos and interactive quizzes on any given topic. Leveraging **AI**, it creates engaging content, synthesizes speech, and provides a structured learning experience.

---

## ✨ Features

- 📚 **Topic-Based Content Generation** – Input a topic and generate relevant educational content.
- 🎥 **Video Creation** – Synthesizes speech and combines it with a background image.
- 📝 **Interactive Quizzes** – Tests understanding with MCQs based on the topic.
- 💻 **Dynamic UI** – Smooth and user-friendly interface.

---

## 🛠️ Technologies Used

- **Backend**: Flask (Python Web Framework)  
- **AI Integration**: Google Gemini API  
- **Text-to-Speech**: gTTS (Google Text-to-Speech)  
- **Video Processing**: moviepy  
- **Frontend**: HTML, CSS, JavaScript  
- **Environment Management**: Python `venv`  
- **Dependency Management**: pip  

---

## 📁 Project Structure

- `ai_video.py` – Python script for AI/video generation logic  
- `index.py` – Main server file  
- `static/` – Static assets  
  - `style.css` – Custom styling  
  - `script.js` – JavaScript for interactivity  
  - `background.jpg` – Background image used in videos  
  - `output.mp4` – Generated video (appears here)  
- `templates/` – HTML templates  
  - `index.html` – Main landing page  
  - `video_page.html` – Displays the generated video  
  - `quiz_page.html` – Displays quiz questions  
- `.env` – Stores environment variables (keep secret)  
- `requirements.txt` – Lists Python dependencies  
- `README.md` – This file  

---

## 🧩 Setup and Local Installation

### ✅ Prerequisites

- Python 3.8+
- pip (Python package installer)
- FFmpeg (required for moviepy)

---

### ⚙️ Installation Steps

1. **Clone or open your project folder**

   ```bash
   git clone <your-repo-url>
   cd stuvio_project
   ```

   *Or manually navigate to:*

   ```bash
   cd C:\Users\divya\Downloads\Documents\project
   ```

2. **Create and activate a virtual environment**

   ```bash
   python -m venv venv
   ```

   - **PowerShell**:  
     ```bash
     .\venv\Scripts\Activate.ps1
     ```
   - **CMD**:  
     ```bash
     venv\Scripts\activate.bat
     ```
   - **Linux/macOS**:  
     ```bash
     source venv/bin/activate
     ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Configure environment variables**

   Create a `.env` file in the root directory with:

   ```
   GEMINI_API_KEY="your_actual_gemini_api_key"
   FLASK_SECRET_KEY="your_secret_key_here"
   ```

---

## 🚀 Running the Application

Start the Flask server:

```bash
python api/index.py
```

Then open your browser and go to:
[http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 🧪 Usage Guide

1. Enter a **topic** on the homepage.
2. Click **Generate Video** or **Generate Quiz**.
3. Wait for the system to process it.
4. The results will appear on a new page.

---

## ⚠️ Notes

- Video generation time depends on input length.
- FFmpeg **must** be installed and properly added to `PATH`.
- Check your terminal logs for errors if something fails.
- Be mindful of **Gemini API usage limits** and potential charges.

---
▶️ [Watch demo video](https://drive.google.com/file/d/18kVZHTxKGZMKAdPtbcNRjF_z3bCV-1O6/view)

