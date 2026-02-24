# Drowsiness_detection-system
# DrowsyGuard — Driver Drowsiness Detection

🔗 **Live Demo:** [harshita-vk.github.io/Drowsiness_detection-system](https://harshita-vk.github.io/Drowsiness_detection-system/)

---

## What is this?

We built this for an **Ideathon at NMIT College**. We are 2nd year BE Computer Science students and this was our first time building something real with computer vision.

The idea was simple — drowsy driving causes a lot of accidents and we wanted to build something that could actually help. The system watches your eyes through the webcam and triggers an alarm if it detects that you've been closing your eyes for too long while driving.

---

## How it works

It uses something called the **Eye Aspect Ratio (EAR)**. It tracks 6 points around each eye and calculates a ratio. When your eyes are open the ratio is high, when they start closing it drops. If it stays low for too many frames in a row, the alarm goes off.

We originally built it in Python using OpenCV and MediaPipe. But then we thought — what's the point if only people with Python installed can use it? So we converted the whole thing to run in the browser using JavaScript. Now anyone can just open the link and use it, no installation needed.

---

## Tech used

- MediaPipe FaceMesh — facial landmark detection
- WebRTC — webcam access in the browser
- HTML5 Canvas — drawing the eye tracking overlay on the video
- Web Audio API — alarm sound (no external audio file needed)
- Vanilla JavaScript — all the detection logic

No backend. No server. Runs 100% in the browser.

---

## Features

- Live webcam feed with glowing eye landmarks drawn on top
- Real-time EAR value shown on screen
- Alarm triggers when drowsiness is detected
- Tracks total drowsy events in a session
- Adjustable sensitivity with sliders
- Works directly in the browser — nothing to install

---

## Known limitations

- Doesn't work well in low light
- Can lose face tracking if you move too far from camera
- Mainly tested on laptop webcams

---

## Run it yourself

Just open the link and allow camera permission. Or clone it and open `index.html` in your browser.

```bash
git clone https://github.com/harshita-vk/Drowsiness_detection-system.git
```

---

## Team

2nd year BE Computer Science — NMIT College

**Harshita VK** — [@harshita-vk](https://github.com/harshita-vk)
**Manaswi C** — [@Manawi0718](https://github.com/Manaswi0718)

---

*Built for an ideathon and for learning. Not intended as an actual safety system.*
