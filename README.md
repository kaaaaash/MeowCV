<div>
  <h1>MeowCV 😼</h1>
  <h3>Real-Time Facial Expression → Cat Reaction Engine</h3>
</div>

<p>
  A lightweight real-time computer vision system that maps human facial expressions 
  to viral cat reactions using OpenCV + MediaPipe.
</p>

<p>
  <img src="https://github.com/kaaaaash/MeowCV/blob/main/assets/cat-disgust.jpeg" width="380">
</p>

---

## ✨ Overview

MeowCV is a rule-based real-time facial expression engine that tracks 468 facial landmarks using MediaPipe FaceMesh and applies pure geometric heuristics to resolve expressions into dynamic cat reactions — no machine learning training required.

Built for experimentation, performance benchmarking, and playful computer vision exploration.

---

## 🚀 Core Features

- 🎯 Real-time MediaPipe FaceMesh tracking  
- 🧠 Lightweight heuristic-based expression engine  
- 🔄 Dynamic reaction switching  
- 📊 Live FPS monitoring  
- 🎮 Quick exit controls (`Q` / `ESC`)  
- 🪟 Dual-window rendering (Camera + Reaction)

---

## ⚙️ Architecture

| Stage | Component |
|-------|------------|
| 1 | Webcam Input |
| 2 | MediaPipe FaceMesh |
| 3 | Landmark Distance Engine |
| 4 | Expression Resolver |
| 5 | Cat Reaction Renderer |



Pure geometric logic.  
No deep learning model training.  
No heavy inference pipeline.

---

## 🧪 Supported Expressions

| Expression | Trigger Logic |
|------------|--------------|
| 😱 Shock   | Eye vertical distance increases |
| 👅 Tongue  | Mouth vertical distance increases |
| 😾 Glare   | Eye vertical distance decreases |
| 🐱 Idle    | Default fallback state |

---

## 📊 Performance

FPS is calculated per frame and rendered live:

```python
fps = 1 / (current_frame_time - prev_frame_time)
```

Useful for evaluating performance under varying lighting conditions and hardware configurations.

🛠 Setup
----
Python Version

```
Python 3.10 is required.
Python 3.13+ is not supported due to MediaPipe compatibility constraints.
```
Installation
----
### 1. Clone the repository
```
git clone https://github.com/kaaaaash/MeowCV.git
cd MeowCV
```


### 2. Install dependencies
Python **3.9 – 3.12** required (tested on Python 3.10). Python **3.13+** is not supported for `mediapipe==0.10.14`.
```bash
pip install -r requirements.txt
```
▶️ Run
----
```bash
python main.py
```

<div align='center'><h3>
Camera launches.<br>
Expression tracking activates.<br>
Cats respond instantly.
</h3></div>

---
## 🎛 Configuration


All sensitivity thresholds are configurable inside main.py:
```
eye_opening_threshold = 0.020
mouth_open_threshold = 0.030
squinting_threshold = 0.016
```

Adjust values based on lighting conditions and camera quality.

## 🔮 Roadmap

- Expression smoothing<br>
- Animated reaction overlays<br>
- Modular engine structure<br>
- Web-based version (WebRTC)<br>
- Plugin-style reaction packs<br>

## 📜 License

MIT License

Copyright (c) 2026 Shana Nursoo<br>
Copyright (c) 2026 Aaroh Seth

<div align="center">
  <sub>
    Nothing here is broken.<br>
    That’s the problem.
  </sub>
</div>
