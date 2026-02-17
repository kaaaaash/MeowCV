MeowCV v2 😼
Real-Time Facial Expression → Cat Reaction Engine
A lightweight real-time facial expression engine built with OpenCV + MediaPipe that maps human expressions to viral TikTok cat reactions.
Now with performance monitoring, instant exit controls, and cleaner internal logic.
<img src="https://github.com/kaaaaash/MeowCV/blob/main/assets/cat-disgust.jpeg" width="340"> 
________________________________________
🧠 What’s New in v2
•	✅ Improved threshold tuning
•	✅ Real-time FPS counter
•	✅ Instant quit controls (Q / ESC)
•	✅ Cleaner expression priority logic
•	✅ More stable MediaPipe version handling
v2 focuses on usability, performance visibility, and cleaner engineering decisions.
________________________________________
⚙️ System Overview
Pipeline:
Webcam → FaceMesh → Landmark Extraction → Heuristic Engine → Cat Renderer
Detection Logic
Expressions are triggered using geometric relationships between landmarks:
•	Shock → Eye vertical distance exceeds threshold
•	Tongue → Mouth vertical distance exceeds threshold
•	Glare → Eye vertical distance below squint threshold
•	Idle → Default state
No ML training required — purely rule-based detection.
________________________________________
🎮 Controls
Key	Action
Q	Quit program
ESC	Quit program
________________________________________
📊 Performance Monitoring
FPS is calculated per frame:
fps = 1 / (current_frame_time - prev_frame_time)
Displayed in real time to:
•	Measure efficiency
•	Assist optimization
•	Monitor system performance
________________________________________
🛠 Installation
Python Version
Use:
Python 3.10 (recommended)
⚠ Python 3.13+ not supported (MediaPipe compatibility).
________________________________________
Setup
git clone https://github.com/kaaaaash/MeowCV.git
cd MeowCV

py -3.10 -m venv venv
venv\Scripts\activate

pip install mediapipe==0.10.9 opencv-python
________________________________________
Run
python main.py
Camera launches.
Expression tracking begins.
Cats judge accordingly.
________________________________________
🎛 Configuration
All sensitivity thresholds are adjustable in main.py.
eye_opening_threshold = 0.020
mouth_open_threshold = 0.030
squinting_threshold = 0.016
Fine-tune detection responsiveness to match your lighting and camera quality.
________________________________________
🚀 Future Roadmap (v3 Ideas)
•	Expression smoothing (reduce flicker)
•	Animated overlays instead of static images
•	Bounding box UI
•	Web-based version (WebRTC)
•	Modular expression engine (/core/expressions.py)
•	Plugin-style cat packs
________________________________________
📜 License
MIT License
Copyright (c) 2026 Shana Nursoo
Copyright (c) 2026 Aaroh Singh
________________________________________
💡 Philosophy
MeowCV v2 proves that expressive CV systems don’t need heavy ML pipelines.
Simple geometry + clean logic + performance awareness = responsive systems.
And also…
cats reacting to your face is elite software design.

