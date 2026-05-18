# 🏋️ Real-Time Voice & Video AI Gym Coach

An AI-powered real-time fitness coach built using **Python, MediaPipe, OpenCV, Streamlit, and Groq AI**.

This application uses **computer vision, pose estimation, and AI-generated voice coaching** to analyze workout posture, count repetitions, detect exercise form, and provide real-time feedback directly through webcam interaction.

---

# 🚀 Features

✅ Real-time pose detection  
✅ AI-powered workout analysis  
✅ Live skeleton tracking  
✅ Real-time repetition counter  
✅ Exercise posture correction  
✅ AI voice-based workout coaching  
✅ Multi-exercise support  
✅ Webcam-based interaction  
✅ Real-time video streaming using WebRTC  
✅ Interactive Streamlit UI  
✅ Workout metrics & feedback system  

---

# 🧠 Supported Exercises

- Squats
- Push-ups
- Biceps Curls (Dumbbell)
- Shoulder Press
- Lunges

---

# 🛠️ Tech Stack

## Frontend / UI
- Streamlit
- Streamlit WebRTC

## AI / Computer Vision
- MediaPipe
- OpenCV
- NumPy

## Backend
- Python

## AI & Voice Services
- Groq API
- gTTS (Google Text-to-Speech)

## Additional Libraries
- Pandas
- python-dotenv

---

# 📦 Dependencies

```txt
streamlit==1.54.0
streamlit-webrtc==0.64.5
mediapipe==0.10.14
opencv-python-headless==4.10.0.84
pandas==2.2.3
groq>=0.12.0
gtts==2.5.3
python-dotenv==1.2.2
```

---

# 📂 Project Structure

```bash
RealTime-Voice-Video-AI-Gym-Coach/
│
├── core/
│   └── base_exercise.py
│
├── detectors/
│   ├── squat.py
│   ├── pushup.py
│   ├── biceps_curl.py
│   ├── shoulder_press.py
│   └── lunges.py
│
├── services/
│   ├── auth/
│   ├── coaching/
│   ├── config/
│   ├── persistence/
│   ├── state/
│   ├── tracking/
│   ├── ui/
│   └── vision/
│
├── static/
│   └── style.css
│
├── ml_models/
│   └── pose_landmarker_full.task
│
├── main.py
├── requirements.txt
├── packages.txt
├── data.db
└── README.md
```

---

# ⚙️ Installation

## 1️⃣ Clone Repository

```bash
git clone https://github.com/nakulcharak002/RealTime-Voice-Video-AI-Gym-Coach.git

cd RealTime-Voice-Video-AI-Gym-Coach
```

---

## 2️⃣ Create Virtual Environment

### Windows

```bash
python -m venv .venv

.venv\Scripts\activate
```

### Mac/Linux

```bash
python3 -m venv .venv

source .venv/bin/activate
```

---

## 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🔐 Environment Variables

Create a `.env` file in the root directory:

```env
GROQ_API_KEY=your_api_key
```

---

# ▶️ Run the Application

```bash
streamlit run main.py
```

---

# 🌐 Live Demo

🚀 Try the application live here:

👉 https://realtime-gym-trainer.streamlit.app/

---

# 📹 Demo Features

The application provides:

- Real-time pose detection
- AI workout analysis
- Rep counting
- AI voice coaching
- Skeleton tracking
- Posture correction
- Live webcam interaction

directly inside the browser.

---

# 🧠 How It Works

1. Webcam frames are captured in real time.
2. MediaPipe detects 33 human body landmarks.
3. Exercise-specific detectors analyze body movement.
4. Joint angles and posture are calculated.
5. Repetitions are counted automatically.
6. AI voice coaching provides workout feedback.
7. Live overlays are rendered on screen.

---

# 🔥 AI Processing Pipeline

```text
Webcam Feed
      ↓
OpenCV Frame Processing
      ↓
MediaPipe Pose Estimation
      ↓
33 Human Body Landmarks
      ↓
Exercise Detection Logic
      ↓
Rep Counting + Form Analysis
      ↓
AI Voice Feedback
      ↓
Live Video Rendering
```

---

# 💡 AI Concepts Used

- Pose Estimation
- Real-Time Computer Vision
- Human Landmark Detection
- Motion Tracking
- Exercise Form Analysis
- AI Voice Feedback Systems

---

# 📸 Screenshots

## Home Screen

```md
![Home Screen](assets/home.png)
```

## Live Pose Detection

```md
![Pose Detection](assets/pose_detection.png)
```

---

# ☁️ Streamlit Deployment

Deploy easily using Streamlit Community Cloud:

👉 https://share.streamlit.io

## Deployment Steps

1. Push project to GitHub
2. Open Streamlit Cloud
3. Connect GitHub repository
4. Select:
   - Repository: `RealTime-Voice-Video-AI-Gym-Coach`
   - Main File: `main.py`
5. Click **Deploy**

---

# ⚠️ Streamlit Deployment Fix

Create a `packages.txt` file for OpenCV & MediaPipe support.

## packages.txt

```txt
libgl1
libglib2.0-0
```

---

# 🚀 Future Improvements

- Workout history dashboard
- Calorie tracking
- Personalized workout plans
- Multi-person pose tracking
- Mobile app support
- Advanced AI fitness analytics
- Wearable device integration

---

# 👨‍💻 Author

### Nakul Rajput

GitHub:  
https://github.com/nakulcharak002

---

# 📜 License

This project is licensed under the MIT License.

---

# ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!
