FocusLink
A productivity and mental-wellness web app designed to help students stay organized, focused, and emotionally supported while working on academic or personal projects. FocusLink blends project management, timed focus sessions, task tracking, and AI-generated mental-health check-ins to create a supportive workflow experience.
Project Description
FocusLink allows users to create projects, add tasks, track progress, and log focus sessions using a built-in timer system. Each project displays its progress visually and stores a history of productivity sessions.
A key feature of FocusLink is the Mental Health Check-In, where users record their mood and optional notes. The app uses AI-generated supportive responses to promote emotional well-being, motivation, and stress relief, making productivity more sustainable and human-centered.
FocusLink is built with Flask, HTML/CSS, JavaScript, and OpenAI API integration for generating mental-health responses.
How to Use the App
Home Page
Create a new project by entering a project name.
Click on any listed project to open its dashboard.
Project Dashboard
Add tasks and mark them as complete.
Watch your progress bar update in real time.
Use the focus session timer by selecting duration and mood, then start the countdown.
Log focus sessions automatically.
Mental Health Check-In
Choose a mood and optionally write notes.
The app will generate a supportive AI response tailored to your entry.
All check-ins are saved and displayed in the log.
How to Launch the App Locally
1. Clone the repository
git clone <your-repo-url>
cd focuslink
2. Create a virtual environment
python3 -m venv venv
source venv/bin/activate
3. Install dependencies
pip install -r requirements.txt
4. Set your OpenAI API key
export OPENAI_API_KEY="your-key-here"
5. Run the app
python app.py
The app will run at:
http://127.0.0.1:5000
Common Issues You Might Encounter
Issue: OpenAI API key not loading
Make sure you exported it in the same terminal you're running the app.
Use echo $OPENAI_API_KEY to verify it's set.
Issue: "openai" module not found
Install it manually:
pip install openai
Issue: CSS or templates not loading
Ensure the structure looks like this:
focuslink/
│ app.py
│ requirements.txt
│ README.md
│
├── static/
│   └── style.css
│
└── templates/
    ├── index.html
    └── project.html
